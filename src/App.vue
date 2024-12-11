<script setup>
import Header from './components/Header.vue';
import Card from './components/Card.vue';
//import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <!--обёртка для всего содержимого, чтобы прижать footer к нижней части-->
  <div class="wrapper wrapper-forcontent">
    <!--Содержимое сайта без подвала (нужно для прижатия подвала к нижней части)-->
    <div class="content-without-footer">
      <!--Шапка сайта-->
      <Header />
      <!--Основная часть-->
      <main class="main">
        <section class="main-section1">
          <figure class="main-section1-info">
            <div class="main-section1-info-wrap">
              <figure class="main-section1-info-information">
                <div class="main-section1-info-information-wrap--txt">
                  <img src="./assets/images/minilogo.jpg" alt="minilogo" class="main-section1-info-information-minilogo" width="122" height="33">
                  <span class="main-section1-info-information-surprise">Фильтр масла<br>в подарок</span>
                  <button class="main-section1-info-information-details">
                    <span>подробнее</span>
                    <svg width="39" height="22" viewBox="0 0 39 22" xmlns="http://www.w3.org/2000/svg">
                      <path d="M0 10.0833H35.1739L26.9043 1.45176L28.4783 0L39 11L28.4783 22L27.0435 20.5652L35.1739 11.9167H0V10.0833Z"/>
                    </svg>
                  </button>
                </div>
                <div class="main-section1-info-information-wrap--txt">
                  <div class="main-section1-info-information-wrap--txt-btn">
                    <button class="main-section1-info-information-btn">
                      <svg width="34" height="24" viewBox="0 0 34 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M34 11H4.17391L13.1953 1.58374L11.4783 0L0 12L11.4783 24L13.0435 22.4348L4.17391 13H34V11Z"/>
                      </svg>
                    </button>
                    <button class="main-section1-info-information-btn">
                      <svg width="34" height="24" viewBox="0 0 34 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M0 11H29.8261L20.8047 1.58374L22.5217 0L34 12L22.5217 24L20.9565 22.4348L29.8261 13H0V11Z"/>
                      </svg>
                    </button>
                  </div>
                  <span class="main-section1-info-information-span">New Energy</span>
                </div>
              </figure>
              <figure class="main-section1-info-cards"></figure>
            </div>
          </figure>
          <figure class="main-section1-products">
            <Card />
            <figure class="main-section1-products-card">
              <img src="./assets/images/oilbg.png" alt="oilbg" width="297" height="464" class="main-section1-products-card-oilbg">
              <span class="main-section1-products-card-num">02</span>
              <div class="main-section1-products-card-wrap">
                <span class="main-section1-products-card-title">Бесплатный подбор</span>
                <p class="main-section1-products-card-description">Мы найдем самую низкую цену на оригинальную запчасть, достойную альтернативу или самый дешевый аналог.</p>
                <button class="main-section1-products-card-btn">Заявка на подбор</button>
              </div>
            </figure>

            <figure class="main-section1-products-card">
              <span class="main-section1-products-card-num">03</span>
              <div class="main-section1-products-card-wrap">
                <span class="main-section1-products-card-title">Бесплатная доставка</span>
                <p class="main-section1-products-card-description">Согласуем и привезём запчасти в офис или домой в удобное для Вас время.</p>
                <button class="main-section1-products-card-btn">Пункты выдачи</button>
              </div>
            </figure>
          </figure>
        </section>
        <section class="main-section2">
          <figure class="main-section2-promotion1">
            <span class="main-section2-promotion1-title">Щетки<br>AWM</span>
            <button class="main-section2-promotion1-btn">подробнее</button>
          </figure>
          <figure class="main-section2-promotion2">
            <figure class="main-section2-promotion2-info">
              <span class="main-section2-promotion2-info-txt">Весь январь</span>
              <span class="main-section2-promotion2-info-title">скидка 20%<br>на весь<br>DOT4</span>
              <button class="main-section2-promotion2-info-btn">подробнее</button>
            </figure>
            <div class="main-section2-promotion2-slogan">
              <span class="main-section2-promotion2-slogan-txt">Цена снижена</span>
            </div>
          </figure>

        </section>
      </main>
    </div>

    <!--Подвал сайта-->
    <footer class="footer">
      <ul class="footer-list">
        <li class="footer-list-item">Подбор запчастей</li>
        <li class="footer-list-item">Доставка</li>
        <li class="footer-list-item">Как купить</li>
        <li class="footer-list-item">Оплата</li>
        <li class="footer-list-item">Договор оферты</li>
        <li class="footer-list-item">Политика конфиденциальности</li>
        <li class="footer-list-item">Реквизиты</li>
        <li class="footer-list-item">Контакты</li>
        <li class="footer-list-item">Акции</li>
      </ul>
      <div class="footer-buttons-wrap">
        <button class="footer-buttons-btn">
        </button>
        <button class="footer-buttons-btn">
        </button>
        <button class="footer-buttons-btn">
        </button>
      </div>
      <span class="footer-signature">Дизайн — «Есть Идея!»</span>
    </footer>
  </div>
</template>



<style lang="scss" scoped>
@font-face {
    font-family: gothampro700;
    src: url(./assets/fonts/gothampro_bold.ttf);
    font-weight: 700;
    font-style: normal;
}
@font-face {
    font-family: gothampro400;
    src: url(./assets/fonts/gothampro_medium.ttf);
    font-weight: 400;
    font-style: normal;
}
@font-face {
    font-family: gothampro300;
    src: url(./assets/fonts/gothampro_light.ttf);
    font-weight: 300;
    font-style: normal;
}
@font-face {
    font-family: gothampro900;
    src: url(./assets/fonts/gothampro_black.ttf);
    font-weight: 900;
    font-style: normal;
}


/* Переменные (через $) */
$colortext: #ffffff;

*{
  box-sizing: border-box;
}
button:hover{
  cursor: pointer;
}


.main{
  width: 100%;
  padding: 40px 50px 0 50px;
  background-color: #f0f0f0;
  &-section1{
    padding: 0 190px;
    background: url(./assets/images/bgimg.png) no-repeat;
    &-info{
      &-information{
        display: flex;
        justify-content: space-between;
        &-wrap--txt{
          display: flex;
          flex-direction: column;
          &-btn{
            text-align: right;
          }
        }
        &-minilogo{ //мини лого
        margin: 40px 0 35px 0;
        }
        &-surprise{ //фильтр в подарок
          font-family: gothampro700;
          font-size: 42px;
          line-height: 49px;
          color: #ffffff;
        }
        &-details{ // button Подробнее
          width: 163px;
          display: flex;
          margin: 30px 0 40px 0;
          padding: 0;
          color: #222222;
          border: none;
          text-align: left;
          background: none;

          & span{
            margin: 0 16px 0 0;
            padding: 0;
            font-family: gothampro400;
            text-transform: uppercase;  
            font-size: 16px;
            line-height: 24px;
          }
          & svg{
            fill: #1c69d4;
          }
        }
        &-btn{ // right, left
          width: 50px;
          height: 50px;
          border: none;
          background-color: rgba($color: #ffffff, $alpha: 0.2);
          & svg{
            fill: rgba($color: #ffffff, $alpha: 0.2);
          }
          &:hover{
            background-color: rgba($color: #ffffff, $alpha: 0.4);
            & svg{
              fill:#ffffff;
            }
          }
        }
        &-span{ //New Energy
          margin: 67px 0 0 0;
          text-align: right;
          font-family: gothampro300;
          font-size: 75px;
          line-height: 71px;
          color: #ffffff;
        }
      }
    }
    &-products{
      display: flex;
      padding: 0 0 28px 0;
      position: relative;
      z-index: 1;
      &-card{
        max-width: 460px;
        max-height: 216px;
        display: flex;
        padding: 32px 20px 32px 16px;
        background-color: #fff;

        &:nth-child(2){
          margin: 0 30px;
          & img{
            position: absolute;
            z-index: -1;
            bottom: 70px;
            left: 556px;
          }
        }
        &-wrap{
          display: flex;
          flex-direction: column;
          justify-content: space-between;
        }
        &-num{
          font-family: gothampro900;
          font-size: 36px;
          line-height: 36px;
          text-align: center;
          margin: 0 9px 0 0;
          color: rgba($color: #222222, $alpha: 0.33);
        }
        &-title{
          font-family: gothampro700;
          font-size: 24px;
          line-height: 24px;
          text-align: left;
        }
        &-description{
          font-family: gothampro400;
          font-size: 14px;
          line-height: 20px;
          text-align: left;
          padding: 8px 0;
        }
        &-phone{
          font-family: gothampro400;
          font-size: 24px;
          line-height: 40px;
          text-align: left;
        }
        &-btn{
          padding: 13px 103px;
          font-family: gothampro700;
          font-size: 16px;
          line-height: 23px;
          text-align: center;
          border-radius: 4px;
          border: 2px solid #1c69d4;
          color: #1c69d4;
          background: none;
          &:nth-child(4){
            display: flex;
            flex-direction: row;
            padding: 13px 82px;
            border: 2px solid #3ca255;
            color: #3ca255;
            & svg{
              fill: #3ca255;
              margin: 0 8px 0 0;
            }
            & span{
              white-space: nowrap;
              padding: 5px 0 0 0;
            }
          }
        }
      }
    }
  }
  &-section2{
    padding: 0 190px 28px 190px;
    display: flex;
    color: #ffffff;
    &-promotion1{
      width: 460px;
      height: 356px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      margin: 0 30px 0 0;
      padding: 40px;
      background: url(./assets/images/promotion1.jpg) no-repeat;
      &-title{
        margin: 0 0 180px 0;

        font-family: gothampro700;
        font-size: 16px;
        line-height: 24px;
        text-align: left;
      }
      &-btn{
        color: #ffffff;
        padding: 0;
        width: 108px;
        background: none;
        border: none;
        border-bottom: 2px solid #ffffff;


        text-transform: uppercase;
        font-family: gothampro700;
        font-size: 16px;
        line-height: 24px;
        text-align: left;
      }
    }
    &-promotion2{
      width: 950px;
      height: 356px;
      display: flex;
      padding: 40px;
      flex-direction: row;
      justify-content: space-between;
      background: url(./assets/images/promotion2.jpg) no-repeat;

      &-info{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        &-txt{
        font-family: gothampro300;
        font-size: 20px;
        line-height: 24px;
        text-align: left;
        }
        &-title{
          margin: 60px 0;

          font-family: gothampro700;
          font-size: 30px;
          line-height: 36px;
          text-align: left;
        }
        &-btn{
          color: #ffffff;
          padding: 0;
          width: 108px;
          background: none;
          border: none;
          border-bottom: 2px solid #ffffff;


          text-transform: uppercase;
          font-family: gothampro700;
          font-size: 16px;
          line-height: 24px;
          text-align: left;
        }
      }
      &-slogan{
        padding: 13px 15px;
        background-color: #ff4400;
        max-height: 50px;
        &-txt{
          font-family: gothampro400;
          font-size: 15px;
          line-height: 24px;
          text-align:center;

        }
      }
    }
  }
}

.footer{
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 24px 330px;
  background-color: #f0f0f0;
  justify-content: space-between;
    &-list{
    display: flex;
    list-style: none;
    padding: 0;
    &-item{
      font-family: gothampro700;
      font-size: 15px;
      line-height: 19px;
      text-align: center;

      margin: 0 35px 0 0;
      &:nth-last-child(1){
      margin-right: 0;
      }
    }
  }
  &-buttons{
    &-wrap{
      margin: 30px auto 16px auto;
    }
    &-btn{
      height: 30px;
      width: 30px;
      margin: 0 24px 0 0;
      align-items: center;
      border: none;
      border-radius: 24px;
      &:nth-child(1){
        background: #ffffff url(./assets/images/VK.svg) no-repeat center;
        padding: 10px 6px 0 0;
      }
      &:nth-child(2){
        background: #ffffff url(./assets/images/WhatsApp.svg) no-repeat center;
        padding: 0px 0 0 0px;
      }
      &:nth-child(3){
        background: #ffffff url(./assets/images/Instagram.svg) no-repeat center;
      }
      &:nth-last-child(1){
        margin: 0;
      }
    }
  }
  &-signature{
    margin: 0 auto;
    white-space: nowrap;
    font-family: gothampro400;
    font-size: 13px;
    line-height: 19px;
    text-align: center;
  }
}



//<<==================================================================================================================>>


/* === wrapper === */
/* Обёртки - отдельный блок */
.wrapper{
    /*Максимальная ширина страницы и выравнивание содержимого по центру*/
    max-width: 1920px;
    margin: 0 auto;

    //Отступы по краям
    &-container {
        //padding: 0 375px;
        box-sizing: border-box;
    }
    
    /* Обёртка для прижатия подвала к нижней части */
    &-forcontent{
        min-height: 100vh; /* 100 видимых высот */
        display: flex;
        flex-direction: column;
    }
}
/* end === wrapper === end */



/* === content-without-footer === */
/* Основная часть без footer */
.content-without-footer{
    flex-grow:1; /* Отношение блоков */
}
/* end === content-without-footer === end */

</style>
