<template>
  <footer class="container">
    <div class="containerWrap">
      <div class="footAllWrap">
        <div class="footTopWrap">
          <div class="col-3" v-for="(item, index) in footerList" :key="index">
            <ul>
              <li class="cursor-pointer">{{ item.first }}</li>
              <li class="cursor-pointer">{{ item.second }}</li>
              <li class="cursor-pointer">{{ item.third }}</li>
              <li class="cursor-pointer">{{ item.fourth }}</li>
            </ul>
          </div>
        </div>
        <div class="footTopWrap thirdLinks">
          <div class="cursor-pointer">
            <img
              src="https://www.mcdonalds.com/content/dam/sites/tw/apppromo/iosBadge.png"
              alt="apple link"
            />
          </div>
          <div class="cursor-pointer">
            <img
              src="https://www.mcdonalds.com/content/dam/sites/tw/apppromo/androidBadge.png"
              alt="google link"
            />
          </div>
        </div>
        <div class="footBotWrap">
          <div class="smallC">
            <ul class="bot">
              <li class="cursor-pointer">網站使用條款</li>
              <li class="cursor-pointer">隱私權保護聲明</li>
            </ul>
          </div>
          <div class="bot">© 2017 - 2022 McDonald's. 切版練習用.</div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "navbar",
  data() {
    return {
      footerList: [
        {
          first: "關於我們",
          second: "品牌故事與承諾",
          third: "新聞室",
          fourth: "麥當勞季報"
        },
        {
          first: "成為麥胞",
          second: "職涯發展",
          third: "加入我們"
        },
        {
          first: "聯絡我們",
          second: "常見問題"
        },
        {
          first: "麥當勞叔叔之家慈善基金會"
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  margin: 0;
  padding: 0;
}
a {
  text-decoration: none;
}
/* 文字設定 */
span {
  color: #141414;
  font-size: 1.2rem;
  box-sizing: border-box;
  width: fit-content;
}
ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
ul.bot {
  display: flex;
  min-width: 100%;
}
.bot li {
  box-sizing: border-box;
  min-width: 50px;
  padding: 0 5px;
}
div.bot {
  justify-content: end;
}
li {
  text-align: start;
  font-size: 1rem;
  color: rgb(46, 45, 45);
}
li:nth-child(1).cursor-pointer {
  margin-bottom: 8%;
}
.container {
  max-width: 100%;
}
.containerWrap {
  padding: 0 13% 0;
}
.footAllWrap {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.footTopWrap {
  display: flex;
  width: 100%;
  padding: 8% 0 0 0;
}
.footBotWrap {
  display: flex;
  width: 100%;
  justify-content: space-between;
  padding: 2.5rem 0;
}
.thirdLinks {
  padding: 2.5rem 0;
  justify-content: end;
  border-bottom: 0.75px solid grey;
}
.smallC {
  font-size: 1rem;
}
.cursor-pointer {
  cursor: pointer;
}
</style>
