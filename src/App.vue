<script setup>

import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <!--обёртка для всего содержимого, чтобы прижать footer к нижней части-->
  <div class="wrapper wrapper-forcontent">
    <!--Содержимое сайта без подвала (нужно для прижатия подвала к нижней части)-->
    <div class="content-without-footer">
      <!--Шапка сайта-->
      <header class="header">
        <div class="header-mini--info">
          <img src="./assets/images/logo.jpg" alt="logo" class="header-mini--info-img" width="80px" height="88px">
          <div class="header-mini--info-wrap--micro">
            <div class="header-mini--info-wrap--micro-dropdown">
              <button class="header-mini--info-wrap--micro-dropdown-btn">
                Офис на Малиновского
                <svg width="8" height="8" viewBox="0 0 8 8" xmlns="http://www.w3.org/2000/svg">
                  <path d="M0.5 3.5V2.5H1.5V3.5H0.5Z"/>
                  <path d="M2.5 4.5H1.5V3.5H2.5V4.5Z"/>
                  <path d="M3.5 5.5H2.5V4.5H3.5V5.5Z"/>
                  <path d="M4.5 5.5V6.5H3.5V5.5H4.5Z"/>
                  <path d="M5.5 4.5V5.5H4.5V4.5H5.5Z"/>
                  <path d="M6.5 3.5H5.5V4.5H6.5V3.5Z"/>
                  <path d="M6.5 3.5H7.5V2.5H6.5V3.5Z"/>
                </svg>
              </button>
              <ul class="header-mini--info-wrap--micro-dropdown-list">
                <li>new</li>
              </ul>
            </div>
            <button class="header-mini--info-wrap--micro-btn">
              <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <rect x="1" y="4" width="22" height="3" rx="0.7"/>
                <rect x="1" y="16" width="13" height="3" rx="0.7"/>
                <rect x="1" y="10" width="22" height="3" rx="0.7"/>
              </svg>
              <span>Каталог</span>
            </button>
          </div>
        </div>

        <div class="header-search--info">
          <div class="header-wrap--search--info">
            <div class="header-wrap--search--list">
              <span class="header-search--info-phone">8-800-550-19-80</span>
              <ul class="header-search--info-list">
                <li>Подбор запчастей</li>
                <li>Доставка</li>
                <li>Как купить</li>
                <li>Оплата</li>
                <li>Акции</li>
                <li>Контакты</li>
              </ul>
            </div>
            <div class="header-search--info-login">
              <button class="header-search--info-login-btn">
                <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path d="M12.0125 1.93573C9.25545 1.93573 7.01245 4.17873 7.01245 6.93573C7.01245 9.69273 9.25545 11.9357 12.0125 11.9357C14.7695 11.9357 17.0125 9.69273 17.0125 6.93573C17.0125 4.17873 14.7695 1.93573 12.0125 1.93573ZM12.0125 9.93573C10.3585 9.93573 9.01245 8.58973 9.01245 6.93573C9.01245 5.28173 10.3585 3.93573 12.0125 3.93573C13.6665 3.93573 15.0125 5.28173 15.0125 6.93573C15.0125 8.58973 13.6665 9.93573 12.0125 9.93573ZM21.0125 20.9357V19.9357C21.0125 16.0767 17.8715 12.9357 14.0125 12.9357H10.0125C6.15245 12.9357 3.01245 16.0767 3.01245 19.9357V20.9357H5.01245V19.9357C5.01245 17.1787 7.25545 14.9357 10.0125 14.9357H14.0125C16.7695 14.9357 19.0125 17.1787 19.0125 19.9357V20.9357H21.0125Z"/>
                </svg>
                <span >Войти</span>
              </button>
              <button class="header-search--info-login-btn">
                <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path d="M17.8571 4.8V2.4H8.33333V4.8H17.8571ZM7.14286 19.2C6.51139 19.2 5.90578 19.4529 5.45927 19.9029C5.01275 20.353 4.7619 20.9635 4.7619 21.6C4.7619 22.2365 5.01275 22.847 5.45927 23.2971C5.90578 23.7471 6.51139 24 7.14286 24C7.77432 24 8.37993 23.7471 8.82644 23.2971C9.27296 22.847 9.52381 22.2365 9.52381 21.6C9.52381 20.9635 9.27296 20.353 8.82644 19.9029C8.37993 19.4529 7.77432 19.2 7.14286 19.2ZM19.0476 19.2C18.4162 19.2 17.8105 19.4529 17.364 19.9029C16.9175 20.353 16.6667 20.9635 16.6667 21.6C16.6667 22.2365 16.9175 22.847 17.364 23.2971C17.8105 23.7471 18.4162 24 19.0476 24C19.6791 24 20.2847 23.7471 20.7312 23.2971C21.1777 22.847 21.4286 22.2365 21.4286 21.6C21.4286 20.9635 21.1777 20.353 20.7312 19.9029C20.2847 19.4529 19.6791 19.2 19.0476 19.2ZM7.34524 15.3L7.38095 15.156L8.45238 13.2H17.3214C18.2143 13.2 19 12.708 19.4048 11.964L24 3.552L21.9286 2.4H21.9167L20.6071 4.8L17.3214 10.8H8.96428L8.80952 10.476L6.14286 4.8L5.0119 2.4L3.89286 0H0V2.4H2.38095L6.66667 11.508L5.05952 14.448C4.86905 14.784 4.7619 15.18 4.7619 15.6C4.7619 16.2365 5.01275 16.847 5.45927 17.2971C5.90578 17.7471 6.51139 18 7.14286 18H21.4286V15.6H7.64286C7.4881 15.6 7.34524 15.468 7.34524 15.3Z"/>
                </svg>
                <span >Корзина</span>
              </button>
            </div>
          </div>
          <div class="header-search">
            <button class="header-search-btn">
              <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path d="M10.6977 18.3945C12.4739 18.3945 14.1068 17.7835 15.4096 16.7704L19.6394 21L21 19.6395L16.7701 15.4099C17.7843 14.1062 18.3953 12.4734 18.3953 10.6972C18.3953 6.45318 14.9419 3 10.6977 3C6.45336 3 3 6.45318 3 10.6972C3 14.9413 6.45336 18.3945 10.6977 18.3945ZM10.6977 4.92431C13.8816 4.92431 16.4709 7.51347 16.4709 10.6972C16.4709 13.881 13.8816 16.4702 10.6977 16.4702C7.51371 16.4702 4.92441 13.881 4.92441 10.6972C4.92441 7.51347 7.51371 4.92431 10.6977 4.92431Z"/>
              </svg>
            </button>
            <input type="text" class="header-search-inp" placeholder="Что ищите?">
          </div>
        </div>
      </header>

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

                <img src="./assets/images/oilbg.png" alt="oilbg" class="main-section1-info-information-oilbg">

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
            <figure class="main-section1-products-card">
              <span class="main-section1-products-card-num">01</span>
              <div class="main-section1-products-card-wrap">
                <span class="main-section1-products-card-title">Бесплатный звонок</span>
                <p class="main-section1-products-card-description">На любые номера РФ</p>
                <span class="main-section1-products-card-phone">8 800 550-19-80</span>
                <button class="main-section1-products-card-btn">
                  <svg width="30" height="31" viewBox="0 0 30 31" xmlns="http://www.w3.org/2000/svg">
                    <path d="M30 15.1304C30 23.0491 23.407 29.4684 15.2727 29.4684C12.6903 29.4684 10.2643 28.8208 8.15367 27.6843L0 30.2264L2.65833 22.5337C1.31733 20.3733 0.545 17.8393 0.545 15.1304C0.545 7.2117 7.13867 0.79248 15.273 0.79248C23.4077 0.79248 30 7.2117 30 15.1304ZM15.2727 3.0759C8.44467 3.0759 2.89067 8.48358 2.89067 15.1304C2.89067 17.7684 3.767 20.211 5.24933 22.1982L3.70233 26.6747L8.46067 25.1909C10.4157 26.4504 12.7577 27.1849 15.273 27.1849C22.1 27.1849 27.655 21.7779 27.655 15.1307C27.6547 8.4839 22.1003 3.0759 15.2727 3.0759ZM22.7097 18.4326C22.6187 18.2864 22.3783 18.1981 22.0177 18.0225C21.6563 17.8468 19.881 16.9962 19.551 16.8798C19.22 16.7624 18.9787 16.7035 18.7383 17.0551C18.498 17.407 17.806 18.1981 17.595 18.4326C17.3843 18.6677 17.174 18.6972 16.8127 18.5212C16.452 18.3456 15.289 17.9741 13.91 16.7768C12.837 15.8457 12.1123 14.6954 11.9017 14.3435C11.6913 13.992 11.8797 13.802 12.06 13.627C12.2227 13.4694 12.4213 13.2166 12.6017 13.0115C12.7827 12.8061 12.8427 12.6599 12.9623 12.4251C13.0833 12.1906 13.023 11.9856 12.9323 11.8093C12.8423 11.6337 12.1197 9.90425 11.819 9.20078C11.5183 8.49731 11.218 8.61439 11.007 8.61439C10.7967 8.61439 10.5557 8.58496 10.315 8.58496C10.0743 8.58496 9.683 8.67293 9.352 9.02451C9.02133 9.3764 8.089 10.2267 8.089 11.9558C8.089 13.6852 9.382 15.3561 9.563 15.5906C9.74333 15.8247 12.0597 19.4889 15.7297 20.8962C19.4 22.3025 19.4 21.8332 20.062 21.7743C20.7233 21.7158 22.1973 20.9243 22.4993 20.1041C22.7993 19.2826 22.7993 18.5791 22.7097 18.4326Z"/>
                  </svg>
                  <span>+7 (928) 107-80-80</span>
                </button>
              </div>
            </figure>

            <figure class="main-section1-products-card">
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
      </main>
    </div>

    <!--Подвал сайта-->
    <footer>
      
    </footer>
    <span class="footer-title"></span>
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

.header{
  background-color: #ffffff;
  display: flex;
  padding: 26px 55px;
  width: 100%;
  justify-content: space-between;
  &-mini--info{
    display: flex;
    margin: 0 30px 0 0;
    &-wrap--micro{
      margin: 0 30px;
      display: flex;
      flex-direction: column;
      &-dropdown{
        margin: 0 0 18px 0;
        &-btn{
          display: flex;
          padding: 0;
          border: none;
          color: #222222;
          text-align: left;
          background: none;
          & svg{
            margin: 3px 0;
            margin-left: 8px;
            fill: #222222;
          }
        }
        &-list{
          display: none;
          //padding: 0;
          //list-style: none;
        }
        &:hover{
          .header-mini--info-wrap--micro-dropdown-list {display: block;}
          }

      }
      &-btn{
        display: flex;
        padding: 15px 56px;
        border: none;
        color: $colortext;
        border-radius: 4px;
        background-color: #1c69d4;
        & svg{
          fill: $colortext;
        }
        & span{
          padding: 4px 0 0 16px;
        }
      }
    }
  }
  &-search--info{
    display: flex;
    margin: 0;
    flex-direction: column;
    &-phone{
      margin: 0 36px 0 0;
      color: #000;
    }
    &-list{
      display: flex;
      color: #000;
      list-style: none;
      padding: 0;
      & li{
        margin-right: 40px;
        &:nth-last-child(1){
          margin: 0;
        }
      }

    }
    &-login{
      display: flex;
      &-btn{
        display: flex;
        border: none;
        color: #222222;
        background: none;
        & svg{
          fill: #222222;
        }
        & span{
          margin: 4px 0 0 8px;
        }
        &:nth-last-child(1){
          margin: 0 0 0 24px;
        }
      }
    }
  }
  &-search{
    display: flex;
    width: 1397px;
    border: 1px solid #bbbbbb;
    border-radius: 4px;
    padding: 13px 17px;
    margin: 18px 0 0 0;
    box-shadow: inset 0 2px 4px #bbbbbb;
    &-btn{
      border: none;
      background: none;
      margin: 0 8px 0 0;
      & svg{
          fill: #222222;
        }
    }
    &-inp{
      padding: 0;
      border: none;
      background: none;
      vertical-align: top;
      margin: 8px 0;
    }
  }
  &-wrap--search--info{
    display: flex;
    justify-content: space-between;
  }
  &-wrap--search--list{
    display: flex;
  }

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
        }
        &-span{ //New Energy
          margin: 67px 0 0 0;
          text-align: right;
          font-family: gothampro300;
          font-size: 75px;
          line-height: 71px;
          color: #ffffff;
        }
        &-oilbg{
        position: absolute;
        z-index: 0;
        left: 804px;
        top: 215px;
        }
      }
    }
    &-products{
      display: flex;
      padding: 0 0 28px 0;
      position: relative;
      &-card{
        max-width: 460px;
        max-height: 216px;
        display: flex;
        padding: 32px 20px 32px 16px;
        background-color: #fff;

        &:nth-child(2){
          margin: 0 30px;
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
          margin: 0 8px 0 0;
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
