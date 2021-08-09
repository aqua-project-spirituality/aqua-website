<template>
<div>

  <div class="title">
    <div class="one">あなたは一人じゃないよ。</div>
    <div class="two">繋がり</div>
    <div class="three">は大事です。</div>
  </div>
 
  <img class="lp-image" src="https://images.unsplash.com/photo-1545431781-3e1b506e9a37?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80">

  <div class="content">
    <div class="introduction">
      <div class="vision">
        <h1>理念</h1>
        <p>
          <span style="color: gold;">aqua（アクア）</span>は、風の時代・水瓶座の時代の全盛期に向けて、スピリチュアルな旅をしている人や、本当の自分、内なる真実、そして愛を表現したい人のための<span style="text-decoration: underline;">オンライン公共スペース</span>となることを目指します。既存のSNS（ソーシャルメディア）とは異なり、将来的にビットコインのような独自の暗号通貨をプラットフォームに導入することで、スピリチュアルコミュニティの中に国家から独立した社会を構築していきます。これは多くの人にとって、突拍子もなく聞こえるかもしれませんが、今後世界において国の影響力は衰退し、そして私達のテクノロジーは既に、誰でもどんなグループでも信頼が担保された独自の ”私達の” 通貨を創ることができるところまで到達しています。
        </p>
        <p>
          <br><span style="text-decoration: underline;">
            風の時代全盛期に向けて、、、
          </span><br><br>
          風の時代は「コミュニティの時代」とも言われます。風の時代の社会とは、、、今までの地の時代のエネルギーである会社、組織、国家といったトップダウンのピラミッド型の社会構造ではなく、風の水瓶座のエネルギーのような、よりフラットな、社会的ステータスは関係のない、人々が共通の価値観や興味関心で繋がっているネットワーク型（コミュニティ型）の社会です。個人に力と自由が与えられ、その個人個人が自分の“色”、独自性を活かしてお互いに助け合っていく社会です。<span style="color: gold;">aqua（アクア）</span>は、そのような<span style="text-decoration: underline;">近い将来に数多く生まれるであろうコミュニティ型社会</span>の中でも、特にスピリチュアルな事柄に興味関心がある人々のためのプラットフォームを目指します。
        </p>
      </div>
      <p>
        こんにちは、しょうごと申します。僕はプログラマーで、あなたと同じようにスピリチュアルな旅をしている一人です。僕は、上記のようなプラットフォームを実現するための出発点を創っています。<span style="color: gold;">aqua（アクア）</span>というのは、私達の新たな時代と言われている水瓶座の時代 the Age of <span style="color: gold;">Aqua</span>rius に由来します。ここでの自分の活動は、純粋に自分の愛と情熱によるものです。応援していただけると嬉しいです。僕の運命数は一なので、「ゼロからイチ」を創る人生になっています。しかし「イチから無限大」を創るためには、他の人の助けが必要です。皆さんのお力をお貸しください。
      </p>
      <p>
        真実と愛を込めて, <br>
        <a href="https://shogoyamane.com/jp" target="_blank" class="my-name">
          しょうご
        </a>
        <small>— aquaプロジェクト ファウンダー</small>
      </p>
      <small>
        下記のサイトが僕が創っているaquaというスピリチュアルな人々のための新しいSNSです。まだ製作中で、新規登録もできない形にしてますがご参考までに。現状、英語で創ってますが需要があれば日本語でも製作したいと考えています
      </small>
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
  width: 50%;
  font-size: 25px;
  font-family: cursive;
  text-align: center;
}
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
.one {
  color: springgreen;
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
  font-family: cursive;
}
.introduction {
  text-align: center;
  width: 50%;
  margin: 0 auto;
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
  font-style: italic;
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
    font-size: 15px;
  }
  .lp-image {
    width: 100%;
    display: block;
  }
  .introduction p {
    font-size: 14px;
  }
  .infinity-btn {
    width: 96%;
  }
}
</style>