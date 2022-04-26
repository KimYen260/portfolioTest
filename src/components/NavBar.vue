<template>
  <div class="container">
    <div class="containerWrap">
      <div class="navWrap">
        <nav>
          <div class="align-items-end arrWrap">
            <div class="logo">
              <img
                src="https://www.mcdonalds.com/etc/designs/mcd/tw/zh-tw/_jcr_content/logo/image.img.jpg/1649654364979.jpg"
                alt=""
              />
            </div>
            <div class="listWrap">
              <div class="arrList">
                <span>別具滋味</span>
              </div>
              <div class="arrList">
                <span>企業永續</span>
              </div>
              <div class="arrList">
                <span>數位便利</span>
              </div>
              <div class="arrList">
                <span>現正推出</span>
              </div>
              <div class="arrList">
                <span>尋找餐廳</span>
              </div>
            </div>
          </div>
        </nav>
        <div class="navTopWrap">
          <div class="align-items-start arrWrap">
            <div class="arrList">
              <span class="smallC">站內搜尋</span>
            </div>
            <div class="arrList">
              <span class="smallC">我附近的麥當勞</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    msg: String,
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
.smallC {
font-size: 1rem;
}
/* 視窗 */
.container {
  max-width: 100%;
}
/* 視窗內縮 */
.containerWrap {
  padding: 0 13% 0;
  /* border: 1px solid violet; */
}
/* navbar整體排版 */
.navWrap {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
}
/* List頁面排版 div方式*/
.arrWrap {
  display: flex;
  min-width: 100%;
  padding-top: 10px;
  /* border: 2px solid rgb(76, 224, 18); */
}
/* List內容 */
.arrList {
width: 100%;
justify-content: end;
text-align: end;
margin-left: 4%;
}
/* 清單外層 */
.listWrap {
  display: flex;
  min-width: 100%;
  height: 100%;
  padding-bottom: 20px;
}
/* navbar 排版 */
.navTopWrap {
  display: flex;
  width: 30%;
  justify-content: end;
}
.logo{
  box-sizing: border-box;
  max-height: 108px;
  max-width: 108px;

}

</style>
