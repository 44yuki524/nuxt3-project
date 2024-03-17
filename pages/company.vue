<script setup lang="ts">
const SITE_TITLE = "Front Line / Company"
useHead({
    title: SITE_TITLE
});
</script>

<template>
    <div class="company_view"></div>
    <div class="main_contents">
        <ul>
            <li>
                <p>社名</p>
                <p>株式会社 FRONT LINE</p>
            </li>
            <li>
                <p>設立</p>
                <p>20XX.3.18</p>
            </li>
            <li>
                <p>代表</p>
                <p>44yuki 524</p>
            </li>
            <li>
                <p>資本金</p>
                <p>10,000,00JPY</p>
            </li>
            <li>
                <p>所在地</p>
                <p>〒123-4567 三重県津市</p>
            </li>
        </ul>
        <div class="map">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3278.8570736037127!2d136.5076684752558!3d34.73399688142636!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60040cb144fbc061%3A0x4303b87643034e95!2z5rSl6aeF!5e0!3m2!1sja!2sjp!4v1709900502283!5m2!1sja!2sjp" width="600" height="450" style="border:0;" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
</template>

<style scoped>
/* company_view */
    .company_view {
        max-width: 100%;
        height: 250px;
        background-image: url(assets/images/company.png);
        background-position: center;
        background-size: cover;
        margin-top: 80px;
    }

/* main_contents */
    .main_contents {
        max-width: 900px;
        margin-left: auto;
        margin-right: auto;
        margin-top: 100px;
        margin-bottom: 100px;
        font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    }

    .main_contents ul {
        margin-bottom: 100px;
        padding-left: 0px;
    }

    .main_contents ul li  {
        list-style: none;
        display: flex;
        border-bottom: 1px solid #555;
    }

    .main_contents ul li {
        margin-bottom: 20px;
    }

    .main_contents ul li p:nth-child(2) {
        margin-left: 100px;
    }

    .main_contents ul li p:nth-child(1) {
        width: 150px;
        font-weight: bold;
    }

/* map */
    .map {
        max-width: 900px;
    }

    .map iframe {
        width: 100%;
    }

/* resposive */
@media screen and (max-width:750px){
    /* company_view */
    .company_view {
        background-size: contain;
        background-repeat: no-repeat;
        height: 50px;
        margin-top: 50.4px;
    }

    /* main_contents */
    .main_contents {
        margin-top: 50px;
        margin-bottom: 50px;
    }

    .main_contents ul {
        margin-bottom: 50px;
    }

    .main_contents ul li p:nth-child(2) {
        margin-left: 30px;
        font-size: 16px;
    }

    .main_contents ul li p:nth-child(1) {
        width: 80px;
        font-weight: bold;
        padding-left: 20px;
        font-size: 16px;
    }

    /* map */
    .map {
        max-width: 350px;
        margin-left: auto;
        margin-right: auto;
    }

    .map iframe {
        text-align: center;
    }
}
</style>