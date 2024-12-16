<template>
    <figure class="card">
        <span class="card-num" :style="[num == none ? 'display: none' : 'display: block']">{{ num }}</span>
        <div class="card-wrap">
            <span class="card-title">{{ title }}</span>
            <p class="card-description">{{ desc }}</p>
            <span class="card-phone" :style="[phone == none ? 'display: none' : 'display: block']">
                {{ phone }}
            </span>
            <button class="card-btn"
                :style="[btn_img != none ? 'display: flex; flex-direction: row; padding: 13px 82px; border: 2px solid #3ca255; color: #3ca255;' : '']">
                <img class="card-btn-img" src="../assets/images/WhatsAppBtn.svg" alt="btn_img"
                    :style="[btn_img == none ? 'display: none' : 'display: block; margin: 0 8px 0 0;']">
                <span :style="[btn_img != none ? 'white-space: nowrap; padding: 5px 0 0 0;' : '']">{{ btn_text }}</span>
            </button>
        </div>
    </figure>
</template>



<script setup>
defineProps({
    num: {
        type: Number,
        required: true
    },
    title: {
        type: String,
        required: true
    },
    desc: {
        type: String,
        required: true
    },
    phone: {
        type: String,
        required: true
    },
    btn_img: {
        type: String,
        required: true
    },
    btn_text: {
        type: String,
        required: true
    },
});

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




.card {
    max-width: 460px;
    max-height: 216px;
    display: flex;
    padding: 32px 20px 32px 16px;
    background-color: #fff;

    &-wrap {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    &-num {
        font-family: gothampro900;
        font-size: 36px;
        line-height: 36px;
        text-align: center;
        margin: 0 9px 0 0;
        color: rgba($color: #222222, $alpha: 0.33);
    }

    &-title {
        font-family: gothampro700;
        font-size: 24px;
        line-height: 24px;
        text-align: left;
    }

    &-description {
        font-family: gothampro400;
        font-size: 14px;
        line-height: 20px;
        text-align: left;
        padding: 8px 0;
    }

    &-phone {
        font-family: gothampro400;
        font-size: 24px;
        line-height: 40px;
        text-align: left;
    }

    &-btn {
        padding: 13px 103px;
        font-family: gothampro700;
        font-size: 16px;
        line-height: 23px;
        text-align: center;
        border-radius: 4px;
        border: 2px solid #1c69d4;
        color: #1c69d4;
        background: none;
    }
}
</style>