<template>
<div>

  <div class="title">
    <div class="one">You Are Not Alone.</div>
    <div class="two">CONNECTION</div>
    <div class="three">is Important.</div>
  </div>
 
  <img class="lp-image" src="https://images.unsplash.com/photo-1545431781-3e1b506e9a37?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80">

  <div class="content">
    <div class="introduction">
      <div class="vision">
        <p style="color: mediumspringgreen;">
          Hi, my name is Shogo. I was inspired by the message below by a spiritual teacher Teal Swan, and wanted to create a public space for those who are struggling with CONNECTION. You Are Not Alone. Let us make an amazing place to CONNECT. (I'm a programmer and on awakening journey like many of you. I've personally felt lonely for a long time and struggled with connection.)
        <p style="color: magenta; font-style: italic;">
          "Today, I have a message for you.  And that message is, you are not alone.  There has never been a second that you were alone.  There will never be a second that you are alone.  When you came down to this physical life, you came so that source (which is in fact the greater part of you) could come to know itself through your eyes.  You agreed to the perspective of separation so that source could come to know and understand the nature of it's own "oneness" through your eyes.  Perspective is only one angle of truth.  And the real truth is that truth is far more comprehensive than that one angle.  Just because you can't see it, doesn't mean it isn't there.  Remember this when you are observing the stark absence of friendship in your life.  Remember this when you are feeling lonely or misunderstood...  Behind the veil of your limited perspective, we are there.  Your isolation, is merely an illusion.  And by far the greater part of this universe and world not only understands you and not only loves you, but also, IS you."
        </p>
        <p style="color: mediumspringgreen;">
          I've created a social media website that you can enter through the infinity symbol below, so that we can CONNECT each other. I wish this place will be a "home" for those who have felt lonely and resonated with other awakening journeyers. I named this place "aqua" after the Age of "Aqua"rius. Thank you for reading :)
        </p>
      </div>
      <p style="color: mediumspringgreen;">
        Much Love <span>&#128156;</span><span>&#128156;</span><span>&#128156;</span><span>&#129419;</span><span>&#129419;</span><span>&#129419;</span>,<br>Shogo
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
  margin: 60px auto;
  animation: fadeIn 2s linear;
  width: 35%;
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
  margin: 50px auto;
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
    margin: 40px auto;
    width: 95%;
    font-size: 20px;
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