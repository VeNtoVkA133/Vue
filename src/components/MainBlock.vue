<script setup>
import Card from './Card.vue';
</script>


<template>
    <main class="main">
        <section class="main-section1">
            <figure class="main-section1-info">
                <div class="main-section1-info-wrap">
                    <figure class="main-section1-info-information">
                        <div class="main-section1-info-information-wrap--txt">
                            <img src="../assets/images/minilogo.jpg" alt="minilogo"
                                class="main-section1-info-information-minilogo" width="122" height="33">
                            <span class="main-section1-info-information-surprise">Фильтр масла<br>в подарок</span>
                            <button class="main-section1-info-information-details">
                                <span>подробнее</span>
                                <svg width="39" height="22" viewBox="0 0 39 22" xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M0 10.0833H35.1739L26.9043 1.45176L28.4783 0L39 11L28.4783 22L27.0435 20.5652L35.1739 11.9167H0V10.0833Z" />
                                </svg>
                            </button>
                        </div>
                        <div class="main-section1-info-information-wrap--txt">
                            <div class="main-section1-info-information-wrap--txt-btn">
                                <button class="main-section1-info-information-btn">
                                    <svg width="34" height="24" viewBox="0 0 34 24" xmlns="http://www.w3.org/2000/svg">
                                        <path
                                            d="M34 11H4.17391L13.1953 1.58374L11.4783 0L0 12L11.4783 24L13.0435 22.4348L4.17391 13H34V11Z" />
                                    </svg>
                                </button>
                                <button class="main-section1-info-information-btn">
                                    <svg width="34" height="24" viewBox="0 0 34 24" xmlns="http://www.w3.org/2000/svg">
                                        <path
                                            d="M0 11H29.8261L20.8047 1.58374L22.5217 0L34 12L22.5217 24L20.9565 22.4348L29.8261 13H0V11Z" />
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
                <img class="main-section1-products-oilbg" src="../assets/images/oilbg.png" alt="oilbg" width="297"
                    height="464">
                <Card class="main-section1-products-card" num="01" title="Бесплатный звонок" desc="На любые номера РФ"
                    phone="8 800 550-19-80" btn_img="" btn_text="+7 (928) 107-80-80" />

                <Card class="main-section1-products-card" num="02" title="Бесплатный подбор"
                    desc="Мы найдем самую низкую цену на оригинальную запчасть, достойную альтернативу или самый дешевый аналог."
                    btn_text="Заявка на подбор" />

                <Card class="main-section1-products-card" num="03" title="Бесплатная доставка"
                    desc="Согласуем и привезём запчасти в офис или домой в удобное для Вас время."
                    btn_text="Пункты выдачи" />
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

* {
    box-sizing: border-box;
}

button:hover {
    cursor: pointer;
}

@media (min-width: 1920px) {
    .main {

        //display: none;
        width: 100%;
        padding: 40px 50px 0 50px;
        background-color: #f0f0f0;

        &-section1 {
            padding: 0 190px; //calc(calc(100% - 50px) - 89.56%);
            background: url(../assets/images/bgimg.png) no-repeat;

            &-info {
                &-information {
                    display: flex;
                    justify-content: space-between;

                    &-wrap--txt {
                        display: flex;
                        flex-direction: column;

                        &-btn {
                            text-align: right;
                        }
                    }

                    &-minilogo {
                        //мини лого
                        margin: 40px 0 35px 0;
                    }

                    &-surprise {
                        //фильтр в подарок
                        font-family: gothampro700;
                        font-size: 42px;
                        line-height: 49px;
                        color: #ffffff;
                    }

                    &-details {
                        // button Подробнее
                        width: 163px;
                        display: flex;
                        margin: 30px 0 40px 0;
                        padding: 0;
                        color: #222222;
                        border: none;
                        text-align: left;
                        background: none;

                        & span {
                            margin: 0 16px 0 0;
                            padding: 0;
                            font-family: gothampro400;
                            text-transform: uppercase;
                            font-size: 16px;
                            line-height: 24px;
                        }

                        & svg {
                            fill: #1c69d4;
                        }
                    }

                    &-btn {
                        // right, left
                        width: 50px;
                        height: 50px;
                        border: none;
                        background-color: rgba($color: #ffffff, $alpha: 0.2);

                        & svg {
                            fill: rgba($color: #ffffff, $alpha: 0.2);
                        }

                        &:hover {
                            background-color: rgba($color: #ffffff, $alpha: 0.4);

                            & svg {
                                fill: #ffffff;
                            }
                        }
                    }

                    &-span {
                        //New Energy
                        margin: 67px 0 0 0;
                        text-align: right;
                        font-family: gothampro300;
                        font-size: 75px;
                        line-height: 71px;
                        color: #ffffff;
                    }
                }
            }

            &-products {
                display: flex;
                padding: 0 0 28px 0;
                position: relative;
                justify-content: space-between;
                z-index: 1;

                &-oilbg {
                    position: absolute;
                    z-index: -1;
                    top: -282px;
                    left: 563px; //39.934%;//563px;
                }

                &-card {
                    margin-right: 30px;

                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }
            }
        }

        &-section2 {
            padding: 0 190px 28px 190px;
            display: flex;
            color: #ffffff;

            &-promotion1 {
                width: 460px;
                height: 356px;
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                margin: 0 30px 0 0;
                padding: 40px;
                background: url(../assets/images/promotion1.jpg) no-repeat;

                &-title {
                    margin: 0 0 180px 0;
                    font-family: gothampro700;
                    font-size: 16px;
                    line-height: 24px;
                    text-align: left;
                }

                &-btn {
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

            &-promotion2 {
                width: 950px;
                height: 356px;
                display: flex;
                padding: 40px;
                flex-direction: row;
                justify-content: space-between;
                background: url(../assets/images/promotion2.jpg) no-repeat;

                &-info {
                    display: flex;
                    flex-direction: column;
                    justify-content: space-between;

                    &-txt {
                        font-family: gothampro300;
                        font-size: 20px;
                        line-height: 24px;
                        text-align: left;
                    }

                    &-title {
                        margin: 60px 0;
                        font-family: gothampro700;
                        font-size: 30px;
                        line-height: 36px;
                        text-align: left;
                    }

                    &-btn {
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

                &-slogan {
                    padding: 13px 15px;
                    background-color: #ff4400;
                    max-height: 50px;

                    &-txt {
                        font-family: gothampro400;
                        font-size: 15px;
                        line-height: 24px;
                        text-align: center;
                    }
                }
            }
        }
    }
}

@media (max-width: 1920px) {
    .main {

        //display: none;
        width: 100%;
        padding: 40px 50px 0 50px;
        background-color: #f0f0f0;

        &-section1 {
            padding: 0 190px; //calc(calc(100% - 50px) - 89.56%);
            background: url(../assets/images/bgimg.png) no-repeat;

            &-info {
                &-information {
                    display: flex;
                    justify-content: space-between;

                    &-wrap--txt {
                        display: flex;
                        flex-direction: column;

                        &-btn {
                            text-align: right;
                        }
                    }

                    &-minilogo {
                        //мини лого
                        margin: 40px 0 35px 0;
                    }

                    &-surprise {
                        //фильтр в подарок
                        font-family: gothampro700;
                        font-size: 42px;
                        line-height: 49px;
                        color: #ffffff;
                    }

                    &-details {
                        // button Подробнее
                        width: 163px;
                        display: flex;
                        margin: 30px 0 40px 0;
                        padding: 0;
                        color: #222222;
                        border: none;
                        text-align: left;
                        background: none;

                        & span {
                            margin: 0 16px 0 0;
                            padding: 0;
                            font-family: gothampro400;
                            text-transform: uppercase;
                            font-size: 16px;
                            line-height: 24px;
                        }

                        & svg {
                            fill: #1c69d4;
                        }
                    }

                    &-btn {
                        // right, left
                        width: 50px;
                        height: 50px;
                        border: none;
                        background-color: rgba($color: #ffffff, $alpha: 0.2);

                        & svg {
                            fill: rgba($color: #ffffff, $alpha: 0.2);
                        }

                        &:hover {
                            background-color: rgba($color: #ffffff, $alpha: 0.4);

                            & svg {
                                fill: #ffffff;
                            }
                        }
                    }

                    &-span {
                        //New Energy
                        margin: 67px 0 0 0;
                        text-align: right;
                        font-family: gothampro300;
                        font-size: 75px;
                        line-height: 71px;
                        color: #ffffff;
                    }
                }
            }

            &-products {
                position: relative;
                display: flex;
                padding: 0 0 28px 0;    
                justify-content: space-between;
                z-index: 1;

                &-oilbg {
                    position: absolute;
                    z-index: -1;
                    top: -282px;
                    left: 563px; //39.934%;//563px;
                }

                &-card {
                    margin-right: 30px;

                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }
            }
        }

        &-section2 {
            padding: 0 190px 28px 190px;
            display: flex;
            color: #ffffff;

            &-promotion1 {
                width: 460px;
                height: 356px;
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                margin: 0 30px 0 0;
                padding: 40px;
                background: url(../assets/images/promotion1.jpg) no-repeat;

                &-title {
                    margin: 0 0 180px 0;
                    font-family: gothampro700;
                    font-size: 16px;
                    line-height: 24px;
                    text-align: left;
                }

                &-btn {
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

            &-promotion2 {
                width: 950px;
                height: 356px;
                display: flex;
                padding: 40px;
                flex-direction: row;
                justify-content: space-between;
                background: url(../assets/images/promotion2.jpg) no-repeat;

                &-info {
                    display: flex;
                    flex-direction: column;
                    justify-content: space-between;

                    &-txt {
                        font-family: gothampro300;
                        font-size: 20px;
                        line-height: 24px;
                        text-align: left;
                    }

                    &-title {
                        margin: 60px 0;
                        font-family: gothampro700;
                        font-size: 30px;
                        line-height: 36px;
                        text-align: left;
                    }

                    &-btn {
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

                &-slogan {
                    padding: 13px 15px;
                    background-color: #ff4400;
                    max-height: 50px;

                    &-txt {
                        font-family: gothampro400;
                        font-size: 15px;
                        line-height: 24px;
                        text-align: center;
                    }
                }
            }
        }
    }
}

@media (max-width: 1280px) {
    .main {
        padding: 30px;
        &-section1 {
            padding: 0 30px;
            &-products{
                &-oilbg{
                    left: 430px;
                }
            }
            background-position: -270px 0;
        }
        &-section2 {
            padding: 0 30px 24px 30px;
            &-promotion1{
                background-position: -38px 0;
            }
            &-promotion2{
                background-position: -80px 0;
            }
        }
    }
}

@media (max-width: 960px) {
    .main {
        &-section1 {
            padding: 0 20px;
            &-info{
                &-information{
                    &-span{
                        display: none;
                    }
                }
            }
            &-products{
                &-card{
                    margin-right: 20px;
                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }
                &-oilbg{
                    left: 291px;
                }
            }
        }
        &-section2 {
            padding: 0 20px;
            &-promotion1{
                width: 430px;
                height: 252px;
                padding: 30px 40px;
                &-title{
                    margin: 0 0 118px 0;
                }
            }
            &-promotion2{
                width: 430px;
                height: 252px;
                padding: 30px 40px;
                background-position: -17px 0;
                &-info{
                    &-title{
                        margin: 25px 0;
                        font-size: 23px;
                        line-height: 30px;
                    }
                }
                &-slogan{
                    display: none;
                }
            }
        }
    }
}

@media (max-width: 640px) {
    .main {
        padding: 0;
        &-section1{
            background-position: -590px 0;
            &-products{
                flex-direction: column;
                &-card{
                    margin: 0 0 20px 0;
                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }
                &-oilbg{
                    left: 291px;
                }
            }
        }
    }
}

@media (max-width: 320px) {
    .main {
        &-section1{
            padding: 0 10px;
            &-info{
                &-information{
                    &-wrap--txt{
                        &-btn{
                            width: 100px;
                        }
                    }
                }
            }
            &-products{
                &-oilbg{
                    width: 191px;
                    height: 298px;
                    left: 100px;
                }
            }
        }
        &-section2{
            padding: 0 10px;
            flex-direction: column;
            &-promotion1{
                width: 300px;
                height: 252px;
                margin: 0 0 10px 0;
            }
            &-promotion2{
                width: 300px;
                height: 252px;
            }
        }
    }
}
</style>