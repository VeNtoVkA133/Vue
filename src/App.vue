<script setup>
import Header from './components/Header.vue';
import Main from './components/MainBlock.vue';
import Footer from './components/Footer.vue';
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
      <Main />
    </div>

    <!--Подвал сайта-->
    <Footer />
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
