<template>
  <footer class="container">
    <div class="containerWrap">
      <div class="footWrap">
        <div class="cols-4">
          <ul>
            <li>關於我們</li>
            <li>品牌故事與承諾</li>
            <li>新聞室</li>
            <li>麥當勞季報</li>
          </ul>
        </div>
         <div class="cols-4">
          <ul>
            <li>成為麥胞</li>
            <li>職涯發展</li>
            <li>加入我們</li>
          </ul>
        </div>
         <div class="cols-4">
          <ul>
            <li>聯絡我們</li>
            <li>常見問題</li>
          </ul>
        </div>
         <div class="cols-4">
          <ul>
            <li>麥當勞叔叔之家慈善基金會</li>
          </ul>
        </div>
        <div class="footTopWrap">
          
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "navbar",
  data() {
    return {};
  }
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
  /* border: 1px solid violet; */
}
.navWrap {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
}
.arrWrap {
  display: flex;
  min-width: 100%;
  padding-top: 10px;
  /* border: 2px solid rgb(76, 224, 18); */

}
/* 清單外層 */
.listWrap {
  display: flex;
  min-width: 100%;
  height: 100%;
  padding-bottom: 20px;
  
  /* border: 2px solid rgb(182, 10, 197); */

}
.arrList {
width: 100%;
justify-content: end;
text-align: end;
margin-left: 4%;
}

.navTopWrap {
  display: flex;
  width: 30%;
  justify-content: end;
}

.smallC {
font-size: 1rem;
}
</style>
