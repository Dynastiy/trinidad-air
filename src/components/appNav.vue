<template>
  <div>
    <div>
      <div class="container-fluid">
        <div class="app--nav">
          <div class="follow--us">
            <ul class="d-flex" style="gap:30px">
              <li class="d-flex align-items-center" style="gap:8px"><a href="">Follow Us</a>
              <span class="line"></span></li>
              <li>
                <a href="https://twitter.com/trinidadair">
                  <i class="fa fa-twitter" aria-hidden="true"></i>
                </a>
              </li>
              <li>
                <a href="https://instagram.com/Trinidadair">
                  <i class="fa fa-instagram" aria-hidden="true"></i>
                </a>
              </li>
            </ul>
          </div>

          <div class="logo">
           <router-link to="/">  <img src="@/assets/img/icon.png" alt="" /> </router-link>
          </div>

          <div class="nav--area">
            <ul class="d-flex " style="gap:30px">
              <li><a href="/">Home</a></li>
              <li><a href="#about-us">About Us</a></li>
              <li><a href="mailto:mailto:reservations@trinidadair.com">Contact Us</a></li>
            </ul>
          </div>
        </div>

        <div class="mobile--nav">
          <div class="d-flex align-items-center justify-content-between">
            <div class="logo">
           <router-link to="/">  <img src="@/assets/img/logo_spread.png" alt="" width="150px" /> </router-link>
          </div>
          <div>
            <i @click="drawer=!drawer" class="fa fa-bars text-white fa-2x" aria-hidden="true"></i>
          </div>
          </div>

          <el-drawer
            :visible.sync="drawer"
            direction="ltr"
            size="60%">
           <div class="p-5">
            <ul class="d-flex flex-column" style="gap:20px">
              <li><a class="text-dark" href="/">Home</a></li>
              <li><a class="text-dark" href="#about-us">About Us</a></li>
              <li><a class="text-dark" href="mailto:mailto:reservations@trinidadair.com">Contact Us</a></li>
              <li class="d-flex align-items-center text-dark" style="gap:8px"><a class="text-dark" href="">Follow Us</a>
              <span class="line" style="background-color: var(--accent-color-dark)"></span></li>
              <li>
                <a href="https://twitter.com/trinidadair">
                  <i class="fa fa-twitter text-dark" aria-hidden="true"></i>
                </a>
              </li>
              <li>
                <a href="https://instagram.com/Trinidadair">
                  <i class="fa fa-instagram text-dark" aria-hidden="true"></i>
                </a>
              </li>
            </ul>
           </div>
            
          </el-drawer>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      drawer: false,
    }
  }
}
</script>