<script setup lang="ts">
const SITE_TITLE = "Front Line / Message"
useHead({
    title: SITE_TITLE
});
</script>

<template>
    <div class="message_view"></div>
    <div class="main_contents">
        <div class="intro1">
            <h1>『<span class="yellow">web</span>』をきっかけに踏み出そう！</h1>
            <p>応援させてください！</p>
        </div>
        <div class="intro2">
            <div class="myphoto">
                <img src="../assets/images/myphoto.png" alt="myphoto">
            </div>
            <p>はじめまして。代表の<span class="yellow">44yuki</span>です。テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト テキスト</p>
        </div>
        <div class="desk_photo">
            <img src="../assets/images/desk_photo.png" alt="チームワーク画像">
        </div>
    </div>
</template>

<style scoped>
/* message_view */
    .message_view {
        max-width: 100%;
        height: 250px;
        background-image: url(assets/images/message.png);
        background-position: center;
        background-size: cover;
        margin-top: 80px;
    }

/* main_contents */
    .main_contents {
        font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        max-width: 900px;
        margin:100px auto 100px auto;
    }

    .intro1 {
        text-align: center;
        margin-bottom: 40px;
    }

    .intro1 h1 {
        margin: 0;
        margin-bottom: 30px;
    }

    .intro1 p {
        font-weight: bold;
        font-size: 22px;
        margin: 0;
    }

    .intro1 .yellow {
        color: #efe44e;
    }

    .intro2 {
        display: flex;
        padding-left: 50px;
        padding-right: 50px;
    }

    .intro2 img {
        width: 100px;
        margin-right: 20px;
    }

    .intro2 p {
        margin-top: 0px;
        margin-bottom: 0px;

    }

    .intro2 span {
        color: #efe44e;
    }

    .desk_photo {
        margin-top: 60px;
    }

    .desk_photo img {
        max-width: 900px;
    }

/* responsive */
@media screen and (max-width:750px){
    /* message_view */
    .message_view {
        background-size: contain;
        background-repeat: no-repeat;
        height: 50px;
        margin-top: 50.4px;
    }

    /* main_contents */
    .main_contents {
        margin: 50px auto 50px auto;
    }

    .intro1 h1 {
        font-size: 20px;
        margin-bottom: 10px;
    }

    .intro1 p {
        font-size: 18px;
    }

    .intro2 {
        display: block;
        text-align: center;
        padding-left: 10px;
        padding-right: 10px;
    }
    .intro2 p {
        text-align: left;
    }

    .intro2 img {
        margin-right: 0px;
        margin-bottom: 10px;
    }

    .desk_photo {
        margin-top: 20px;
        text-align: center;
    }

    .desk_photo img {
        max-width: 350px;
    }
}


</style>