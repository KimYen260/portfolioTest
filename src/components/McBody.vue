<template>
  <footer class="container">
    <div class="containerWrap">
      <div
        id="carouselExampleSlidesOnly"
        class="carousel slide"
        data-bs-ride="carousel"
      >
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="https://www.mcdonalds.com/is/image/content/dam/tw/carousel/desktop/210519/PCSafety.jpg?$Hero_Desktop$
" class="d-block w-100" alt="slides" />
          </div>
          <div class="carousel-item">
            <img src="https://www.mcdonalds.com/is/image/content/dam/tw/carousel/desktop/2022/0420/mfckorean-carousel-pc-1260x560.jpg?$Hero_Desktop$
" class="d-block w-100" alt="slides" />
          </div>
          <div class="carousel-item">
            <img src="https://www.mcdonalds.com/is/image/content/dam/tw/carousel/desktop/210519/PCSafety.jpg?$Hero_Desktop$
" class="d-block w-100" alt="slides" />
          </div>
          
          
        </div>
      </div>
      <div class="cards">
        <div class="card col-6" style="width: 18rem;">

  <img src="https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$" class="card-img-top" alt="...">
  <div class="card-body">
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
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
