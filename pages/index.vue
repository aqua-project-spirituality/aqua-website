<template>
<div class="container">

  <h2 class="title">
    <span>Let us create</span> the social platform for spiritual community in the Age of Aquarius <span>together</span>
  </h2>
  
  <img class="lp-image" src="https://images.unsplash.com/photo-1545431781-3e1b506e9a37?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80">

  <div class="content">
    <div class="introduction">
      <div class="vision">
        <h1>Vision</h1>
        <p>
          For the coming the age of Aquarius, <span style="color: gold;">aqua</span> is aiming to be an online public space for anybody who is being on their spiritual journey and anybody who wants to express their authenticity, inner truth, and love. Unlike the existing social media, we are going to introduce an original unique currency — a cryptocurrency like Bitcoin — into our platform in the future, so as to build an alternative and independent society within spiritual community. It may sound crazy a bit at first to many people, but our technology has already reached the point where anybody, or any group can create their own currency.
        </p>
      </div>
      <p>
        Hi, my name is Shogo. I'm a programmer and one of those on a spiritual journey like you. I've created the very starting point to manifest such place as described above, called <span class="gold">aqua</span>, deriving from the Age of <span class="gold">Aqua</span>rius —which is known as our new world. Our new world where we are all align with our own higher self.
      </p>
      <p>
        All works here in aqua are purely labor of my love and passion. I appreciate if you support me. I assume aqua will be an important platform for anyone who resonates with spirituality, because our world is heading towards Web3.0 – where a certain group has own unique currency in order to achieve collective social goal. aqua is the first Web3.0 platform specified for spiritual community.
      </p>
      <p>
          My life path number is 1, so I'm supposed to create "Zero to One". But to create "One to Infinity", I need others' help, so please join me. Hope you join me to create an ideal world together.
      </p>
      <p>
        my inner truth and love, <br>
        <a href="https://shogoyamane.com" target="_blank" class="my-name">
          Shogo
        </a>
        <small>— Founder of aqua</small>
      </p>
    </div>
    <button class="btn infinity-btn" @click="infinity">
      <span>&#8734;</span>
    </button>
  </div>
  
</div>
</template>

<script>
export default {
  methods: {
    infinity() {
      const url = 'https://aqua01-1ccd0.web.app'
      window.open(url, '_blank')
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

.title {
  animation: fadeIn 3s linear;
  width: 40%;
  font-family: "Crimson Text", serif;
  font-weight: normal;
  font-size: 25px;
  font-style: italic;
  margin: 60px auto;
  text-align: center;
  color: aqua;
}
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
.title span {
  color: deeppink;
  font-style: initial;
}
.lp-image {
  animation: fadeIn 3s linear;
  width: 90%;
  display: block;
  margin: 50px auto;
}

.content {
  margin: 0px auto;
}
.introduction {
  text-align: center;
  width: 50%;
  margin: 0 auto;
  font-style: italic;
}
.introduction p + p {
  margin: 25px auto;
}
.introduction .gold {
  color: gold;
}
.my-name {
  color: #f2f2f2;
  text-decoration: underline;
}

.vision {
  margin: 50px auto;
  color: mediumspringgreen;
}
.vision p {
  margin: 10px auto;
}

.infinity-btn {
  background-color: #fff;
  display: block;
  margin: 50px auto;
  width: 90%;
  border-radius: 10px;
  box-shadow: 0 0 50px 20px #fff;
  transition: background-color 1s linear;
}
.infinity-btn span {
  font-size: 40px;
  color: gold;
}


@media screen and (max-width: 550px) {
  .introduction {
    width: 80%;
  }
  .title {
    width: 95%;
    font-size: 20px;
    margin: 40px auto;
  }
  .lp-image {
    width: 100%;
    display: block;
  }
  .infinity-btn {
    width: 96%;
  }
}
</style>