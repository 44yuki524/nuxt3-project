<script setup lang="ts">
const SITE_TITLE = "Front Line / Top"
useHead({
    title: SITE_TITLE
});
</script>

<template>
    <div class="firstview"></div>
    <div class="main_contents">
        <div class="news">
            <div class="news_inner">
                <div class="news_title">
                    <img src="../assets/images/NEWS_title.png" alt="news_title">
                </div>
                <div class="news_contents">
                    <ul>
                        <li>
                            <span>20XX.02.10</span>
                            <p>サイトをリニューアルいたしました。</p>
                        </li>
                        <li>
                            <span>20XX.02.08</span>
                            <p>採用強化中です。一緒に働きませんか？？</p>
                        </li>
                        <li>
                            <span>20XX.06.02</span>
                            <div class="news_2line">
                                <p>xx月xx日まで新規登録キャンペーンを開催中!</p>
                                <p>サービス内でつかえるポイントをプレゼント!</p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="service">
            <div class="service_inner">
                <div class="service_title">
                    <img src="../assets/images/SERVICE_title.png" alt="service_title">
                </div>
                <div class="service_contents">
                    <div class="service_item">
                        <img src="../assets/images/webcreate_b.png" alt="Web制作事業">
                    </div>
                    <div class="service_item">
                        <img src="../assets/images/school_b.png" alt="スクール事業">
                    </div>
                    <div class="service_item">
                        <img src="../assets/images/media_b.png" alt="Webメディア事業">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* firstview */
.firstview {
    max-width: 100%;
    height: 600px;
    background-image: url(assets/images/firstview.png);
    background-position: center;
    background-size: cover;
    margin-top: 80px;
}
/* main_contents */
.main_contents {
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

/* news */
.news {
    max-width: 1280px;
    margin-left: auto;
    margin-right: auto;
}

.news_inner {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 100px;
    margin-bottom: 100px;
}
.news ul {
    margin: 0;
    padding-left: 50px;
}

.news li {
    list-style: none;
    border-bottom: 1px solid #555;
    display: flex;
    margin-top: 10px;
}

.news li:first-child {
    margin-top: 0px;
}

.news li p {
    font-weight: bold;
    margin: 0 20px 10px 40px;
    display: inline-block;
    font-size: 20px;
    letter-spacing: 2.0;
}

.news_2line {
    display:flex;
    flex-flow: column;
}

.news_2line p:first-child {
    margin-bottom: 2px;
}

.news_title {
    height: 154px;
}

.news_title img {
    width: 120px;
}

.news_contents span {
    font-size: 18px;
}

/* servoce */
.service {
    max-width: 1280px;
    margin-top: 120px;
    margin-bottom: 120px;
    background-image: url(../assets/images/SERVICE_bg.png);
    background-repeat: no-repeat;
    background-position: 60% 0%;
    margin-left: auto;
    margin-right: auto;
}

.service_title {
    margin-top: 150px;
    margin-bottom: 50px;
    padding-left: 6%;
}

.service_title img {
    width: 170px;
}

.service_contents {
    display: flex;
    justify-content: center;
    align-items: center;
}

.service_item {
    margin-right: 25px;
}

.service_item img {
    width: 350px;
}

/* responsive */
@media screen and (max-width:750px){
    /* firstview */
    .firstview {
        background-size: contain;
        background-repeat: no-repeat;
        height: 150px;
        margin-top: 50.4px;
    }

    /* news */
    .news_inner {
        margin-top: 40px;
        margin-bottom: 40px;
        display: block;
        text-align: center;
    }

    .news ul {
        padding-left: 10px;
        padding-right: 10px;
    }

    .news ul li p {
        font-size: 14px;
        text-align: left;
    }

    .news ul li span {
        font-size: 11px;
    }

    .news_title {
        height: 80px;
    }

    .news_title img {
        width: 100px;
    }

    /* service */
    .service {
        max-width: 250px;
        background-size:contain;
        background-position-y: 15px;
        margin-bottom: 50px;
    }

    .service_title {
        padding-left: 0%;
        margin-bottom: 30px;
        margin-top: 70px;
    }

    .service_inner {
        text-align: center;
    }

    .service_contents {
        display: block;
    }

    .service_item {
        margin-right: 0px;
    }

    .service_item img {
        width: 250px;
    }

    }
</style>
