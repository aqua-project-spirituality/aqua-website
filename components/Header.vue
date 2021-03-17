<template>
  <header class="header">

    <div class="header-container">
      <div class="logo">
        <nuxt-link to="/">
          <h2>
            <span>&#8734;</span><span class="logo-a"> a</span>qua <span>&#8734;</span>
          </h2>
        </nuxt-link>
      </div>
      <div class="moon" @click="showMenu = true">
        <span>&#9789;</span>
      </div>
    </div>

    <!-- menu modal -->
    <div class="modal-cover" 
        v-if="showMenu"
        @click.self="showMenu = false">
      <div class="menu">
        <span class="close" @click="close">x</span>
        <ul>
          <li @click="close"><nuxt-link to="/menu/about">About</nuxt-link></li>
          <li @click="close"><nuxt-link to="/menu/blog">Blog</nuxt-link></li>
          <li @click="close"><nuxt-link to="/menu/learning">Learning</nuxt-link></li>
          <li @click="close"><nuxt-link to="/menu/contact">Contact</nuxt-link></li>          
        </ul>
      </div>
    </div>
    <!-- menu modal -->

  </header>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    close() {
      this.showMenu = false
    }
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
}
ul {
  list-style: none;
  padding: 0;
}
.header {
  height: 65px;
}
.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 55%;
  margin: 0 auto;
}
.logo {
  margin-left: 4%;
}
.logo h2 {
  font-family: 'Times New Roman', Times, serif;
  font-weight: normal;
  color: gold;
  font-size: 32px;
}
.logo-a {
  color: deeppink;
}
.moon {
  cursor: pointer;
  padding: 5px;
  font-size: 32px;
  margin-right: 5%; 
  color: springgreen;
}
.menu {
  box-shadow: 0 0 70px 5px snow;
  background-color: lightyellow;
  border-radius: 50%;
  width: 500px;
  height: 500px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
}
.close {
  color: deeppink;
  cursor: pointer;
  padding: 10px 20px;
  font-size: 18px;
  position: absolute;
  top: 20px;
}
.menu li {
  margin: 15px auto;
  text-align: center;
}
.menu a {
  color: deeppink;
  font-size: 23px;
  display: inline-block;
  width: 100%;
}

/* modal */
.modal-cover {
  z-index: 1;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, .5);
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  animation: fadeIn .3s linear;
}
/* modal */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@media screen and (max-width: 550px) {
  .header-container {
    width: initial;
  }
  .logo h2 {
    font-size: 28px;
  }
  .moon {
    font-size: 28px;
  }
  .menu {
    width: 320px;
    height: 320px;
  }
  .close {
    padding: 5px 10px;
    font-size: 14px;
    top: 5px;
  }
  .menu a {
    font-size: 16px;
  }
}
</style>