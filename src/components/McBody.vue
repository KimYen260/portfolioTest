<template>
  <footer class="container">
    <div class="containerWrap">
      <div class="bodyWrap">
        <div class="footTopWrap">
          <div class="col-3" v-for="(item, index) in footerList" :key="index">
            <ul>
              <li>{{ item.first }}</li>
              <li>{{ item.second }}</li>
              <li>{{ item.third }}</li>
              <li>{{ item.fourth }}</li>
            </ul>
          </div>
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
          fourth: "麥當勞季報",
        },
        {
          first: "成為麥胞",
          second: "職涯發展",
          third: "加入我們",
        },
        {
          first: "聯絡我們",
          second: "常見問題",
        },
        {
          first: "麥當勞叔叔之家慈善基金會",
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

.container {
  max-width: 100%;
}
.containerWrap {
  padding: 0 13% 0;
}
.bodyWrap {
  display: flex;
  flex-direction: column;
  width: 100%;
}


.smallC {
  font-size: 1rem;
}
</style>
