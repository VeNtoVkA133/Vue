<template>
    <footer class="footer">
        <ul class="footer-list">
            <div class="footer-list-first">
                <li class="footer-list-item">Подбор запчастей</li>
                <li class="footer-list-item">Доставка</li>
                <li class="footer-list-item">Как купить</li>
                <li class="footer-list-item">Оплата</li>
                <li class="footer-list-item">Договор оферты</li>
            </div>
            <div class="footer-list-second">
                <li class="footer-list-item second-item">Политика конфиденциальности</li>
                <li class="footer-list-item second-item">Реквизиты</li>
                <li class="footer-list-item second-item">Контакты</li>
                <li class="footer-list-item second-item">Акции</li>
            </div>
            
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
</template>




<script setup>


</script>




<style lang="scss" scoped>
@media (min-width: 1920px) {
    .footer {
        width: 100%;
        //display: none;
        display: flex;
        flex-direction: column;
        padding: 24px 330px;
        background-color: #f0f0f0;
        justify-content: space-between;

        &-list {
            display: flex;
            list-style: none;
            padding: 0;
            &-first{
                display: flex;
                flex-direction: row;
            }
            &-second{
                display: flex;
                flex-direction: row;
            }
            &-item {
                font-family: gothampro700;
                font-size: 15px;
                line-height: 19px;
                text-align: center;
                white-space: nowrap;

                margin: 0 35px 0 0;

                &:nth-last-child(1) {
                    margin-right: 0;
                }
            }
        }

        &-buttons {
            &-wrap {
                margin: 30px auto 16px auto;
            }

            &-btn {
                height: 30px;
                width: 30px;
                margin: 0 24px 0 0;
                align-items: center;
                border: none;
                border-radius: 24px;

                &:nth-child(1) {
                    background: #ffffff url(../assets/images/VK.svg) no-repeat center;
                    padding: 10px 6px 0 0;
                }

                &:nth-child(2) {
                    background: #ffffff url(../assets/images/WhatsApp.svg) no-repeat center;
                    padding: 0px 0 0 0px;
                }

                &:nth-child(3) {
                    background: #ffffff url(../assets/images/Instagram.svg) no-repeat center;
                }

                &:nth-last-child(1) {
                    margin: 0;
                }
            }
        }

        &-signature {
            margin: 0 auto;
            white-space: nowrap;
            font-family: gothampro400;
            font-size: 13px;
            line-height: 19px;
            text-align: center;
        }
    }
}

@media (max-width: 1920px) {
    .footer {
        width: 100%;
        //display: none;
        display: flex;
        flex-direction: column;
        padding: 24px 330px;
        background-color: #f0f0f0;
        justify-content: space-between;

        &-list {
            display: flex;
            list-style: none;
            padding: 0;
            &-first{
                display: flex;
                flex-direction: row;
                margin: 0 35px 0 0;
            }
            &-second{
                display: flex;
                flex-direction: row;
            }
            &-item {
                font-family: gothampro700;
                font-size: 15px;
                line-height: 19px;
                text-align: center;
                white-space: nowrap;

                margin: 0 35px 0 0;

                &:nth-last-child(1) {
                    margin-right: 0;
                }
            }
        }

        &-buttons {
            &-wrap {
                margin: 30px auto 16px auto;
            }

            &-btn {
                height: 30px;
                width: 30px;
                margin: 0 24px 0 0;
                align-items: center;
                border: none;
                border-radius: 24px;

                &:nth-child(1) {
                    background: #ffffff url(../assets/images/VK.svg) no-repeat center;
                    padding: 10px 6px 0 0;
                }

                &:nth-child(2) {
                    background: #ffffff url(../assets/images/WhatsApp.svg) no-repeat center;
                    padding: 0px 0 0 0px;
                }

                &:nth-child(3) {
                    background: #ffffff url(../assets/images/Instagram.svg) no-repeat center;
                }

                &:nth-last-child(1) {
                    margin: 0;
                }
            }
        }

        &-signature {
            margin: 0 auto;
            white-space: nowrap;
            font-family: gothampro400;
            font-size: 13px;
            line-height: 19px;
            text-align: center;
        }
    }
}

@media (max-width: 1440px) {
    .footer {
        width: 100%;
        padding: 24px 70px;
    }
    .second-item{
        &:nth-child(2){
            display: none;
        }
    }
}

@media (max-width: 1280px) {
    .footer {
        width: 100%;
        padding: 24px 52px;
    }
    .second-item{
        &:nth-child(1){
            display: none;
        }
        &:nth-child(2){
            display: none;
        }
    }
}

@media (max-width: 960px) {
    .footer {
        width: 100%;
        padding: 24px 23px;
        &-list{
            display: flex;
            flex-direction: column;
            white-space: nowrap;
            &-first{
                display: flex;
                flex-direction: row;
            }
            &-second{
                display: flex;
                flex-direction: row;
                margin: 20px 31px 0 31px;
            }
        }
    }
}



@media (max-width: 640px) {
    .footer {
        width: 100%;
        padding: 24px 10px;
        align-self: flex-start;
        &-list{
            display: flex;
            flex-direction: column;
            white-space: nowrap;
            &-first{
                display: flex;
                flex-direction: column;
                & li{
                    align-self: flex-start;
                }
            }
            &-second{
                display: flex;
                flex-direction: column;
                //margin: 20px 31px 0 31px;
                & li{
                    align-self: flex-start;
                }
            }
        }
        &-buttons{
            &-wrap{
                margin: 20px 0 0 10px;
            }
        }
        &-signature{
            margin: 16px 0 0 10px;
        }
    }
}
</style>