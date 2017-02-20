<template>
  <div class="hello">
    <p class="world skew">{{ msg }}</p>
    <div class="original"></div>
    <div class="relative"></div>
    <div class="next"></div>

    <section>
      <a class="cmn-t-colour">Colour</a>
    </section>

    <section>
      <a class="cmn-t-bg">Background</a>
    </section>

    <section>
      <a class="cmn-t-radius">Border Radiu</a>
    </section>

    <section>
      <a class="cmn-t-scale">scale</a>
    </section>
    <div class="news content">
      Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Donec ornare vulputate mi. Nullam auctor pede sit amet odio varius consectetuer. Fusce bibendum neque eu purus. Donec et nulla at odio volutpat luctus. Cras facilisis consequat nisi. Aliquam erat volutpat. Etiam tellus magna, ultrices quis, porttitor non, bibendum quis, lacus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Sed felis. Phasellus enim. Aliquam malesuada mi eu erat. Suspendisse potenti. In diam ante, sagittis vel, rutrum at, fringilla pulvinar, nunc.著作权归作者所有。
      商业转载请联系作者获得授权,非商业转载请注明出处。
      原文: http://www.w3cplus.com/content/css-selection © w3cplus.com
    </div>
  </div>

</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: '世界'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .hello, .relative, .original, .next{
    box-sizing: border-box;
  }

  section {
    margin: 0 0 20px 0;
    text-align: center;
  }

  section a {
    display: inline-block;
    font-size: 16px;
    transition: all 0.2s
  }
  .cmn-t-colour {
    position: relative;
    width: 100px;
    color: #ff3296;;
  }

  .cmn-t-colour:hover {
    color: #98004a;
    font-size: 30px;
  }

  .cmn-t-bg {
    background-color: #ff3296;
    color: #ffffff;
    padding: 20px 30px;
  }

  .cmn-t-bg:hover {
    background-color: #98004a;
    color: #ffffff
  }

  .cmn-t-radius {
    background-color: #ff3296;
    color: #fff;
    padding: 20px 30px;
  }

  .cmn-t-radius:hover {
    background-color: #98004a;
    border-radius: 40px;
  }

  .cmn-t-scale {
    position: relative;
    background-color: #ff3296;
    color: #fff;
    padding: 20px 30px;

  }

  .cmn-t-colour:after {
    position: absolute;
    left:0;
    bottom: -10px;
    content: ' ';
    width: 0;
    height: 10px;
    background-color: #98004a;
    transition: width .2s;
  }

  .cmn-t-colour:hover {
    width: 100%;
  }

  @keyframes pulse {
    0% {
      width: 0;
    }

    50% {
      width: 50%;
    }

    100% {
      width: 100%;
    }
  }

  .world {
    height: 32px;
    color: #333;
    font-size: 32px;
    line-height: 32px;
    -webkit-box-reflect: below 100px
    -webkit-gradient(linear, left top, left bottom, from(transparent),
      to(rgba(255, 255, 255, 0.51)));

  }

  @-webkit-keyframes animl {
    0% {
      font-size: 12px;
    }
    100% {
      font-size: 50px;
    }
  }
  .skew {
    -webkit-animation-name: animl;
    -webkit-animation-duration: 3s;
    -webkit-animation-iteration-count: 4;
    -webkit-animation-direction: alternate;
    -webkit-animation-timing-function: ease-in-out;
  }


  .original {
    width: 60px;
    height: 60px;
    background-color: #0b97c4;
  }

  .relative {
    padding: 20px;
    width: 60px;
    height: 60px;
    border: solid 2px orangered;
  }

  .next {
    cursor: pointer;
       width: 60px;
       height: 60px;
       background-color: #f8d5d8;
     }
  .next:hover {
    background: #0b97c4;
  }
  .next:active {
    background-color: #cc0000;
  }
  .news {
    width: 80px;
    margin: 100px auto 0 auto;
    padding: 20px;
    text-align: left;
    border: 2px solid #00d6b2;
    backgroud:-webkit-gradient(radial,50 50,50,50 1,0,from(black),to(white));
    word-wrap: break-word;
  }

  P:hover {

  }

  .content {
  }
</style>
