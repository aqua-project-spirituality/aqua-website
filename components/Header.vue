<template>
  <header class="header">

    <div class="header-container">

      <div class="logo">
        <nuxt-link to="/" class="header-title">
          <span>&#8734;</span>
            <span class="logo-a"> a</span>qua 
          <span>&#8734;</span>
        </nuxt-link>
      </div>

    </div>

  </header>
</template>

<script>
export default {
  data() {
    return {
      
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
.logo a {
  font-size: 34px;
}
.header-title {
  font-family: fantasy, cursive, Times, serif;
  color: gold;
  outline: none;
}
.logo-a {
  color: deeppink;
}

@media screen and (max-width: 550px) {
  .header-container {
    width: initial;
  }
  .logo a {
  font-size: 28.5px;
  }
}
</style>