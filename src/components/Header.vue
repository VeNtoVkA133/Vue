<template>
    <header class="header">
        <div class="header-mini--info">
            <img src="../assets/images/logo.jpg" alt="logo" class="header-mini--info-img" width="80px" height="88px">
            <div class="header-mini--info-wrap--micro">
                <div class="header-mini--info-wrap--micro-lgw">
                    <figure class="header-mini--info-wrap--micro-logo">
                        <svg width="22" height="15" viewBox="0 0 22 15" fill="none" xmlns="http://www.w3.org/2000/svg"
                            class="header-mini--info-wrap--micro-logo-svg">
                            <rect width="22" height="3" rx="0.7" fill="#222222" />
                            <rect y="12" width="22" height="3" rx="0.7" fill="#222222" />
                            <rect y="6" width="22" height="3" rx="0.7" fill="#222222" />
                        </svg>
                        <span class="header-mini--info-wrap--micro-logo-txt">trlm.ru</span>
                    </figure>
                    <Dropdown class="header-mini--info-wrap--micro-dropdown" />
                    <Login class="header-mini--info-wrap--micro-login" />
                </div>
                <button class="header-mini--info-wrap--micro-btn">
                    <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <rect x="1" y="4" width="22" height="3" rx="0.7" />
                        <rect x="1" y="16" width="13" height="3" rx="0.7" />
                        <rect x="1" y="10" width="22" height="3" rx="0.7" />
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
                <Login class="header-wrap--search--info-login" />
            </div>
            <div class="header-search">
                <button class="header-search-btn">
                    <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M10.6977 18.3945C12.4739 18.3945 14.1068 17.7835 15.4096 16.7704L19.6394 21L21 19.6395L16.7701 15.4099C17.7843 14.1062 18.3953 12.4734 18.3953 10.6972C18.3953 6.45318 14.9419 3 10.6977 3C6.45336 3 3 6.45318 3 10.6972C3 14.9413 6.45336 18.3945 10.6977 18.3945ZM10.6977 4.92431C13.8816 4.92431 16.4709 7.51347 16.4709 10.6972C16.4709 13.881 13.8816 16.4702 10.6977 16.4702C7.51371 16.4702 4.92441 13.881 4.92441 10.6972C4.92441 7.51347 7.51371 4.92431 10.6977 4.92431Z" />
                    </svg>
                </button>
                <input type="text" class="header-search-inp" placeholder="Что ищите?">
            </div>
        </div>
    </header>
</template>



<script setup>
import Dropdown from './Dropdown.vue';
import Login from './Login.vue';
</script>



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
    .header {
        background-color: #ffffff;
        display: flex;
        padding: 26px 55px;
        width: 100%;
        justify-content: space-between;

        &-mini--info {
            display: flex;
            margin: 0 30px 0 0;

            &-wrap--micro {
                margin: 0 0 0 30px;
                display: flex;
                flex-direction: column;

                &-login {
                    display: none;
                }

                &-logo {
                    display: none;
                }

                &-btn {
                    display: flex;
                    padding: 15px 56px;
                    border: none;
                    color: $colortext;
                    border-radius: 4px;
                    background-color: #1c69d4;

                    & svg {
                        fill: $colortext;
                    }

                    & span {
                        padding: 4px 0 0 16px;
                    }



                    &:hover {
                        background-color: #2681ff;
                    }

                    &:active {
                        background-color: #0055cb;
                    }
                }
            }
        }

        &-search--info {
            display: flex;
            margin: 0;
            width: 1397px;
            flex-direction: column;
            white-space: nowrap;

            &-phone {
                margin: 0 36px 0 0;
                color: #000;
            }

            &-list {
                display: flex;
                color: #000;
                list-style: none;
                padding: 0;

                & li {
                    margin-right: 40px;

                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }

            }

            &-login {
                display: flex;

                &-btn {
                    display: flex;
                    border: none;
                    color: #222222;
                    background: none;

                    & svg {
                        fill: #222222;
                    }

                    & span {
                        margin: 4px 0 0 8px;
                    }

                    &:nth-last-child(1) {
                        margin: 0 0 0 24px;
                    }
                }
            }
        }

        &-search {
            display: flex;
            width: 100%;
            border: 1px solid #bbbbbb;
            border-radius: 4px;
            padding: 13px 17px;
            margin: 18px 0 0 0;
            box-shadow: inset 0 2px 4px #bbbbbb;

            &-btn {
                border: none;
                background: none;
                margin: 0 8px 0 0;

                & svg {
                    fill: #222222;
                }
            }

            &-inp {
                padding: 0;
                border: none;
                background: none;
                vertical-align: top;
                margin: 8px 0;
            }
        }

        &-wrap--search--info {
            display: flex;
            justify-content: space-between;
        }

        &-wrap--search--list {
            display: flex;
        }

    }
}

@media (max-width: 1920px) {
    .header {
        background-color: #ffffff;
        display: flex;
        padding: 26px 55px;
        width: 100%;
        justify-content: space-between;

        &-mini--info {
            display: flex;
            margin: 0 30px 0 0;

            &-wrap--micro {
                margin: 0 0 0 30px;
                display: flex;
                flex-direction: column;

                &-login {
                    display: none;
                }

                &-logo {
                    display: none;
                }

                &-btn {
                    display: flex;
                    padding: 15px 56px;
                    border: none;
                    color: $colortext;
                    border-radius: 4px;
                    background-color: #1c69d4;
                    font-family: gothampro700;
                    font-size: 16px;
                    line-height: 23px;


                    & svg {
                        fill: $colortext;
                    }

                    & span {
                        padding: 4px 0 0 16px;
                    }



                    &:hover {
                        background-color: #2681ff;
                    }

                    &:active {
                        background-color: #0055cb;
                    }
                }
            }
        }

        &-search--info {
            display: flex;
            margin: 0;
            width: 1397px;
            flex-direction: column;
            white-space: nowrap;

            &-phone {
                margin: 0 36px 0 0;
                color: #000;
            }

            &-list {
                display: flex;
                color: #000;
                list-style: none;
                padding: 0;

                & li {
                    margin-right: 40px;

                    &:nth-last-child(1) {
                        margin: 0;
                    }
                }

            }

        }

        &-search {
            display: flex;
            width: 100%;
            border: 1px solid #bbbbbb;
            border-radius: 4px;
            padding: 13px 17px;
            margin: 18px 0 0 0;
            box-shadow: inset 0 2px 4px #bbbbbb;

            &-btn {
                border: none;
                background: none;
                margin: 0 8px 0 0;

                & svg {
                    fill: #222222;
                }
            }

            &-inp {
                padding: 0;
                border: none;
                background: none;
                vertical-align: top;
                margin: 8px 0;
            }
        }

        &-wrap--search--info {
            display: flex;
            justify-content: space-between;
        }

        &-wrap--search--list {
            display: flex;
        }

    }
}

@media (max-width: 1280px) {
    .header {
        padding: 23px 30px;

        &-mini--info {
            margin: 0 20px 0 0;
        }

        &-search--info {
            &-list {
                & li:nth-child(3) {
                    display: none;
                }
            }
        }
    }
}

@media (max-width: 960px) {
    .header {
        padding: 23px 20px;

        &-search--info {
            &-list {
                display: none;
            }
        }
    }
}

@media (max-width: 640px) {
    .header {
        &-mini--info {
            &-img {
                display: none;
            }

            &-wrap--micro {
                margin: 0;

                &-lgw {
                    display: flex;
                    flex-direction: row;
                    margin: 0 0 10px 0;
                }

                &-logo {
                    display: flex;
                    margin: 0 18px 0 0;

                    &-svg {
                        margin: 0 9px 0 0;
                    }

                    &-txt {
                        font-family: gothampro700;
                        font-size: 16px;
                        line-height: 23px;
                        text-align: left;
                    }
                }
            }
        }
    }
}

@media (max-width: 320px) {
    .header {
        padding: 10px;

        &-search--info {
            display: none;
        }

        &-search {
            display: none;
        }

        &-mini--info {
            margin: 0;

            &-wrap--micro {

                justify-content: space-between;

                &-lgw {
                    flex-direction: row;
                    justify-content: space-between;
                }

                &-logo {
                    &-svg {
                        margin: 4px 9px 0 0;
                    }
                }

                &-dropdown {
                    display: none;
                }

                &-login {
                    display: flex;
                }

                &-btn {
                    padding: 15px 97px;

                    & span {
                        padding: 0 0 0 16px;
                    }
                }
            }
        }
    }
}
</style>