<template>
  <div class="container">
    <div class="containerWrap">
      <div
        id="carouselExampleSlidesOnly"
        class="carousel slide overflow-hidden"
        data-bs-ride="carousel"
      >
        <div class="carousel-inner col-10">
          <div class="carousel-item active">
            <img
              src="https://s7d1.scene7.com/is/image/mcdonalds/PCSafety:accessible-carousel-desktop"
              class="d-block w-100"
              alt="slides"
            />
            <!-- fixed card -->
            <div class="card cardPosi">
              <div class="card-body">
                <h2 class="card-title">麥當勞餐廳相關公告</h2>
                <p class="card-text cardPs">
                  即日起， 進入麥當勞餐廳前請配戴口罩、測量額溫與實聯制登記。
                </p>
                <button type="button" class="btn btn-warning btn-lg cardH">
                  了解更多
                </button>
              </div>
            </div>
          </div>
          <div class="carousel-item">
            <img
              src="https://www.mcdonalds.com/content/dam/sites/tw/carousel/desktop/%E5%AE%98%E7%B6%B2PC%202336X1040(new).png"
              class="d-block w-100"
              alt="slides"
            />
            <div
              class="card cardPosi"
            >
              <div class="card-body">
                <h2 class="card-title">【韓風炸鷄腿】韓國直送 熱銷推薦</h2>
                <p class="card-text cardPs">
                  去年錯過？沒關係他又回來了！韓國直送不倒翁甜辣醬，甜辣完美比例，配上多汁鷄腿，想吃就點韓風炸鷄腿
                </p>
                <button type="button" class="btn btn-warning btn-lg cardH">
                  了解更多
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="cards cardWrap"
        v-for="(item, index) in cardList"
        :key="index"
      >
        <div class="card" style="margin-right: 1%">
          <img
            :src="item.first.cardImg"
            class="card-img-top"
            alt="card photo"
          />
          <div class="card-body p-5">
            <h3>{{ item.first.cardTitle }}</h3>
            <p class="card-text cardP">{{ item.first.cardDes }}</p>
            <button type="button" class="btn btn-warning btn-lg cardH">
              {{ item.first.buttonName }}
            </button>
          </div>
        </div>

        <div class="card" style="margin-left: 1%">
          <img
            :src="item.second.cardImg"
            class="card-img-top"
            alt="card photo"
          />
          <div class="card-body p-5">
            <h3>{{ item.second.cardTitle }}</h3>
            <p class="card-text cardP">{{ item.second.cardDes }}</p>
            <button type="button" class="btn btn-warning btn-lg cardH">
              {{ item.second.buttonName }}
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
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
              "https://s7d1.scene7.com/is/image/mcdonalds/what-hot-PC-1:1-2-full-bleed-tile-desktop",
            cardTitle: "現正推出",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
          second: {
            cardImg:
              "https://s7d1.scene7.com/is/image/mcdonalds/mcd-home-mds-pc-1:1-2-full-bleed-tile-desktop",
            cardTitle: "24hr歡樂送",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
        },
        {
          first: {
            cardImg:
              "https://s7d1.scene7.com/is/image/mcdonalds/McCafe-banner:1-2-full-bleed-tile-desktop",
            cardTitle: "一杯McCafé一段對話",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
          second: {
            cardImg:
              "https://s7d1.scene7.com/is/image/mcdonalds/%E8%A6%AA%E5%AD%90%E6%99%82%E5%85%89KV_PC:1-2-full-bleed-tile-desktop",
            cardTitle: "親子時光",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
        },
        {
          first: {
            cardImg:
              "https://s7d1.scene7.com/is/image/mcdonalds/good-food-parents-child:1-2-full-bleed-tile-desktop",
            cardTitle: "安心品質",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
          second: {
            cardImg:
              "https://s7d1.scene7.com/is/image/mcdonalds/Home_Banner_Digital_PC:1-2-full-bleed-tile-desktop",
            cardTitle: "數位便利",
            cardDes:
              "想了解麥當勞有哪些最新活動嗎？你不想錯過的美食、最即時的優惠內容... 馬上探索、馬上行動！",
            buttonName: "了解更多",
          },
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
button {
  margin: 2%;
  box-sizing: border-box;
  padding: 2% 3%;
  font-size: 1rem;
  font-weight: 200;
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
.carousel-item{
 position: relative;
}
.card-img-top.cardH {
  max-height: 60%;
}
.card-text.cardPs {
  text-align: start;
  padding: 2% 1%;
}
.card-text.cardP {
  margin: 1% 0;
}
.cardH {
  padding: 2% 6%;
}
.card {
  box-shadow: 5px 5px 5px rgb(219, 219, 219, 0.3);
}
.cardPosi {
  width: 25rem;
  position: absolute;
  bottom: 20%;
  left: 4%;
  padding: 2% 4%;
}

.smallC {
  font-size: 1rem;
}
</style>
