<template>
  <div class="container">
    <div class="containerWrap">
      <div class="navWrap">
        <nav class="navbar">
          <div class="align-items-center navWrap">
            <div
              class="logo"
              style="
                border: 3px solid red;
                box-sizing: border-box;
                max-height: 108px;
                max-width: 108px;
              "
            >
              <img
                src="https://www.mcdonalds.com/etc/designs/mcd/tw/zh-tw/_jcr_content/logo/image.img.jpg/1649654364979.jpg"
                alt=""
              />
            </div>
            <div class="navWrap">
              <div  style="border: 1px solid red">
                <span>別具滋味</span>
              </div>
              <div  style="border: 1px solid red">
                <span>企業永續</span>
              </div>
              <div  style="border: 1px solid red">
                <span>數位便利</span>
              </div>
              <div  style="border: 1px solid red">
                <span>現正推出</span>
              </div>
              <div  style="border: 1px solid red">
                <span>尋找餐廳</span>
              </div>
            </div>
          </div>
        </nav>
        <div
        style="
                border: 3px solid green;
                box-sizing: border-box;
                justify-content: flex-end;
                max-height: 30px;
                width: auto;
              ">
          <div class="align-items-start navTopWrap">
            <div style="border: 1px solid red">
              <span>站內搜尋</span>
            </div>
            <div style="border: 1px solid red">
              <span>我附近的麥當勞</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "McDonald",
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
span {
  color: #141414;
  font-size: 20px;
}
.container {
  max-width: 100%;
}
.containerWrap {
  padding: 0 13% 0;
  border: 1px solid violet;
}
.navWrap {
  display: flex;
  flex-direction: row;
  margin: 0 0 0 10%;
  border: 1px solid black;
}
.navTopWrap {
  display: flex;
  justify-content: end;
  text-align: end;
}
</style>
