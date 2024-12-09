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
        <figure class="main-info">
          <div class="main-info-wrap">
            <figure class="main-info-information">
              <div class="main-info-information-wrap--txt">
                <img src="./assets/images/minilogo.jpg" alt="minilogo" class="main-info-information-minilogo">
                <span class="main-info-information-surprise">Фильтр масла в подарок</span>
                <button class="main-info-information-details">
                  подробнее
                  <svg width="39" height="22" viewBox="0 0 39 22" xmlns="http://www.w3.org/2000/svg">
                    <path d="M0 10.0833H35.1739L26.9043 1.45176L28.4783 0L39 11L28.4783 22L27.0435 20.5652L35.1739 11.9167H0V10.0833Z"/>
                  </svg>
                </button>
              </div>
            </figure>
            <figure class="main-info-cards"></figure>
          </div>
        </figure>
        <figure class="main-products">

        </figure>
      </main>
    </div>

    <!--Подвал сайта-->
    <footer>
      
    </footer>
    <span class="footer-title"></span>
  </div>
</template>



<style lang="scss" scoped>

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
  background-image: url();
  &-info{
    padding: 0 190px;
    background: url(./assets/images/bgimg.png);
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
