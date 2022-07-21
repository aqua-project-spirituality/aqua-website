<template>
<div>

  <div class="title">
    <div class="one">Dear Spiritual Community...</div>
    <div class="two">Let us build an alternative society</div>
    <div class="three">in the Age of Aquarius.</div>
  </div>
 
  <img class="lp-image" src="https://images.unsplash.com/photo-1545431781-3e1b506e9a37?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80">

  <iframe class="lp-video" width="560" height="315" src="https://www.youtube-nocookie.com/embed/BHrGaKc9OD8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
  </iframe>

  <div class="content">
    <div class="introduction">

      <div class="vision">
        <h1>Vision</h1>
        <p>
          For the coming the age of Aquarius, <span style="color: gold;">aqua</span> is aiming to be an online public space for anybody who is being on their spiritual journey and anybody who wants to express their authenticity, inner truth, and love.
        </p>
        <p>
          Unlike the existing social media, we are going to introduce our own unique currency —a cryptocurrency like Bitcoin— into our platform in the future, so as to build an alternative and independent society within spiritual community. Our technology has already reached the point where anybody and any groups can create their own currency.
        </p>
      </div>

      <p>
        Hi, my name is Shogo. I'm a programmer and one of those on a spiritual journey like you. I've been creating the very starting point to manifest such place as described above, called <span style="color: gold;">aqua</span>, deriving from the Age of <span style="color: gold;">Aqua</span>rius —which is known as our new world. Our new world where we are all align with our own higher selves.
      </p>
      <p>
        All works here in <span style="color: gold;">aqua</span> are purely labor of my love and passion. I appreciate if you support me. I assume <span style="color: gold;">aqua</span> will be an important platform for anyone who resonates with spirituality, because our whole world is heading towards Web3.0 – where a certain group has own unique currency in order to achieve collective social goal. <span style="color: gold;">aqua</span> is the first Web3.0 platform specified for spiritual community.
      </p>
      <p>
        My life path number is 1, so I'm supposed to create "Zero to One". But to create "One to Infinity", I need others' help, so please join me.
      </p>
      <p>
        My inner truth and love, <br>
        <a href="https://shogoyamane.com" target="_blank" class="my-name">
          Shogo
        </a>
        <small>— Founder of aqua project</small>
      </p>
      <p style="color: aqua;">
        The following is a web app that I've been creating for a while. I plan to introduce our unique currency into this app in the future as a reward mechanism. Users who create good contents for others are supposed to get rewarded with the currency, for example.
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
      const url = 'https://aqua01-1ccd0.web.app/'
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
  margin: 60px auto;
  animation: fadeIn 2s linear;
  font-size: 25px;
  font-family: 'Times New Roman', Times, serif;
  text-align: center;
}
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
.one {
  color: mediumspringgreen;
}
.two {
  color: magenta;
}
.three {
  color: aqua;
}

.lp-image {
  animation: fadeIn 2s linear;
  width: 90%;
  display: block;
  margin: 50px auto;
}
.lp-video {
  display: block;
  margin: 0 auto;
}
.content {
  margin: 0px auto;
}
.introduction {
  text-align: center;
  width: 50%;
  margin: 0 auto;
}
.introduction p + p {
  margin: 25px auto;
}
.vision {
  color: mediumspringgreen;
  margin: 50px auto;
}
.vision p {
  margin: 10px auto;
  font-style: italic;
}
.my-name {
  color: #f2f2f2;
  text-decoration: underline;
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
    margin: 40px auto;
    width: 95%;
    font-size: 20px;
  }
  .lp-image {
    width: 100%;
  }
  .lp-video {
    width: 100%;
  }
  .infinity-btn {
    width: 96%;
  }
}
</style>