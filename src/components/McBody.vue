<template>
  <footer class="container">
    <div class="containerWrap">
      <div
        id="carouselExampleSlidesOnly"
        class="carousel slide overflow-hidden"
        data-bs-ride="carousel"
      >
        <div class="carousel-inner col-10">
          <div class="carousel-item active">
            <img
              src="https://www.mcdonalds.com/is/image/content/dam/tw/carousel/desktop/210519/PCSafety.jpg?$Hero_Desktop$"
              class="d-block w-100"
              alt="slides"
            />
          </div>
          <div class="carousel-item">
            <img
              src="https://www.mcdonalds.com/is/image/content/dam/tw/carousel/desktop/2022/0420/mfckorean-carousel-pc-1260x560.jpg?$Hero_Desktop$"
              class="d-block w-100"
              alt="slides"
            />
          </div>
        </div>
      </div>
      <div
        class="cards cardWrap"
        v-for="(item, index) in cardList"
        :key="index"
      >
        <div style="margin-right: 1%">
          <div class="card" style="height:40%">
            <img :src="item.first.cardImg" class="card-img-top" alt="card photo" />
            <div class="card-body p-1">
              <h3>{{ item.first.cardTitle }}</h3>
              <p class="card-text">
                {{ item.first.cardDes }}
              </p>
              <button type="button" class="btn btn-warning btn-lg">{{ item.first.buttonName }}</button>
            </div>
          </div>
        </div>
        <div class="card" style="margin-left: 1%">
          <img :src="item.second.cardImg" class="card-img-top" alt="card photo" />
          <div class="card-body p-1">
            <h3>{{ item.second.cardTitle }}</h3>
            <p class="card-text">
              {{ item.second.cardDes }}
            </p>
            <button type="button" class="btn btn-warning btn-lg">{{ item.second.buttonName }}</button>
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
      cardList: [
        {
          first: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "瞭解更多",
          },
          second: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "瞭解更多",
          },
        },
        {
          first: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
          second: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
        },
        {
          first: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
          second: {
            cardImg:
              "https://www.mcdonalds.com/is/image/content/dam/tw/featured-callout/desktop/zh-tw/what-hot-PC.jpg?$FC_One_By_Two$",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          }
        }
      ]
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
.cardWrap {
  width: 100%;
  padding: 8% 0 0 0;
  display: flex;
  justify-content: space-between;
}
.carousel.slide {
  height: 540px;
  /* border: 10px solid red; */
}
.card.col-6 {
}
.smallC {
  font-size: 1rem;
}
</style>
