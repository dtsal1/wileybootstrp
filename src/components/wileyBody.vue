<template>
    <div class="hero-banner">
        <app-slides></app-slides>
        <!--<div class="simple-responsive-banner-component hero-banner-component">-->
            <!--<div class="carousel-default">-->
                <!--<div class="carousel-gallery">-->
                    <!--<div class="carousel">-->
                        <!--<div class="owl-carousel hero-banner-carousel owl-loaded owl-drag" data-component-model="{&quot;items&quot;:1,&quot;loop&quot;:true,&quot;center&quot;:true,&quot;nav&quot;:true,&quot;navText&quot;:&quot;&quot;,&quot;dots&quot;:true}" style="padding: 0px;">-->

                            <!--<div class="owl-stage-outer">-->
                                <!--<div class="owl-stage" style="transition: all 0s ease 0s; width: 6995px; transform: translate3d(-2798px, 0px, 0px);"><div class="owl-item cloned" style="width: 1399px; background-image: url(../assets/Telescope_desktop.jpg);">-->
                                    <!--<div class="item">-->
                                <!--<div class="item-inner ">-->
                                    <!--<div class="simple-responsive-banner-component">-->
                                        <!--<img class="responsive-image js-responsive-image" alt="Telescope-mobile.jpg" title="Telescope-mobile.jpg" src="../assets/Telescope_desktop.jpg" style="display: none;">-->
                                    <!--</div>-->
                                    <!--<div class="container">-->
                                        <!--<article class="page-section">-->
                                            <!--<div class="wiley-slogan"><div class="banner-heading">Building a Better Future</div><p class="banner-heading-text">Through Education, Skill Development and Research</p></div>-->
                                            <!--<a href="https://www.wiley.com/en-ru/aboutus" class="link-button transparent" title="Learn more">Learn more</a></article>-->
                                    <!--</div>-->
                                <!--</div>-->
                            <!--</div>-->
                            <!--</div><div class="owl-item cloned" style="width: 1399px; background-image: url(../assets/Telescope_desktop.jpg);"><div class="item">-->
                                <!--<div class="item-inner ">-->
                                    <!--<div class="simple-responsive-banner-component">-->
                                        <!--<img class="responsive-image js-responsive-image" alt="Telescope-mobile.jpg" title="Telescope-mobile.jpg" src="../assets/Telescope_desktop.jpg" style="display: none;">-->
                                    <!--</div>-->
                                    <!--<div class="container">-->
                                        <!--<article class="page-section">-->
                                            <!--<div class="wiley-slogan"><div class="banner-heading">Building a Better Future</div><p class="banner-heading-text">Through Education, Skill Development and Research</p></div>-->
                                            <!--<a href="https://www.wiley.com/en-ru/aboutus" class="link-button transparent" title="Learn more">Learn more</a></article>-->
                                    <!--</div>-->
                                <!--</div>-->
                            <!--</div></div><div class="owl-item active center" style="width: 1399px; background-image: url(../assets/Telescope_desktop.jpg);"><div class="item">-->
                                <!--<div class="item-inner ">-->
                                    <!--<div class="simple-responsive-banner-component">-->
                                        <!--<img class="responsive-image js-responsive-image" alt="Telescope-mobile.jpg" title="Telescope-mobile.jpg" src="../assets/Telescope_desktop.jpg" style="display: none;">-->
                                    <!--</div>-->
                                    <!--<div class="container">-->
                                        <!--<article class="page-section">-->
                                            <!--<div class="wiley-slogan"><div class="banner-heading">Building a Better Future</div><p class="banner-heading-text">Through Education, Skill Development and Research</p></div>-->
                                            <!--<a href="https://www.wiley.com/en-ru/aboutus" class="link-button transparent" title="Learn more">Learn more</a></article>-->
                                    <!--</div>-->
                                <!--</div>-->
                            <!--</div></div><div class="owl-item cloned" style="width: 1399px; background-image: url(../assets/Telescope_desktop.jpg);"><div class="item">-->
                                <!--<div class="item-inner ">-->
                                    <!--<div class="simple-responsive-banner-component">-->
                                        <!--<img class="responsive-image js-responsive-image" alt="Telescope-mobile.jpg" title="Telescope-mobile.jpg" src="../assets/Telescope_desktop.jpg" style="display: none;">-->
                                    <!--</div>-->
                                    <!--<div class="container">-->
                                        <!--<article class="page-section">-->
                                            <!--<div class="wiley-slogan"><div class="banner-heading">Building a Better Future</div><p class="banner-heading-text">Through Education, Skill Development and Research</p></div>-->
                                            <!--<a href="https://www.wiley.com/en-ru/aboutus" class="link-button transparent" title="Learn more">Learn more</a></article>-->
                                    <!--</div>-->
                                <!--</div>-->
                            <!--</div></div><div class="owl-item cloned" style="width: 1399px; background-image: url(../assets/Telescope_desktop.jpg);"><div class="item">-->
                                <!--<div class="item-inner ">-->
                                    <!--<div class="simple-responsive-banner-component">-->
                                        <!--<img class="responsive-image js-responsive-image" alt="Telescope-mobile.jpg" title="Telescope-mobile.jpg" src="../assets/Telescope_desktop.jpg" style="display: none;">-->
                                    <!--</div>-->
                                    <!--<div class="container">-->
                                        <!--<article class="page-section">-->
                                            <!--<div class="wiley-slogan"><div class="banner-heading">Building a Better Future</div><p class="banner-heading-text">Through Education, Skill Development and Research</p></div>-->
                                            <!--<a href="https://www.wiley.com/en-ru/aboutus" class="link-button transparent" title="Learn more">Learn more</a></article>-->
                                    <!--</div>-->
                                <!--</div>-->
                            <!--</div></div></div></div><div class="owl-nav disabled"><a tabindex="0" class="owl-prev"></a><a tabindex="0" class="owl-next"></a></div><div class="owl-dots disabled"><div class="owl-dot active"><span></span></div></div></div>-->
                    <!--</div>-->
                <!--</div>-->
            <!--</div></div>-->
        <!--<div class="container">-->
        <!--</div>-->
    </div>
</template>

<script>
    import slides from "./slides"
    export default {
        name: "wileyBody",
     components: {
        appSlides: slides
     }
    }
</script>

<style scoped>
    .wiley-rich-content-page .carousel-default {
        margin: 0;
    }

    .wiley-rich-content-page .simple-responsive-banner-component.hero-banner-component {
        margin: 0;
    }

    .wiley-rich-content-page p {
        margin-bottom: 20px;
        font-size: 16px;
    }

    .wiley-rich-content-page .page-title h2 {
        color: rgba(0, 0, 0, 0.87);
        text-align: left;
    }

    .wiley-rich-content-page .component-wrapper {
        margin-bottom: 20px;
        margin-top: 20px;
    }

    .wiley-rich-content-page .component-wrapper .container-fluid {
        padding: 0;
    }

    .wiley-rich-content-page .page-content-wrapper {
        padding-top: 0px;
    }

    .wiley-rich-content-page .wiley-slogan {
        color: white;
    }

    .wiley-rich-content-page .wiley-slogan h1 {
        color: white;
        font-family: 'Source Serif Pro', serif;
        line-height: 63px;
        font-size: 50px;
        font-weight: 600;
        margin: 0;
    }

    .wiley-rich-content-page .wiley-slogan p {
        color: white;
        font-size: 24px;
        line-height: 30px;
    }

    .wiley-rich-content-page .wiley-slogan p:nth-of-type(1) {
        margin-bottom: 10px;
    }

    .wiley-rich-content-page .wiley-slogan .link-button {
        margin-bottom: 45px;
    }

    .wiley-rich-content-page .hero-banner .container {
        display: block;
        min-height: 0;
    }

    .carousel-default .hero-banner-carousel {
        color: white;
        height: 360px;
        padding: 0;
    }

    .carousel-default .hero-banner-carousel .owl-nav {
        z-index: 2;
        display: block;
    }

    .carousel-default .hero-banner-carousel .owl-nav .owl-next,
    .carousel-default .hero-banner-carousel .owl-nav .owl-prev {
        width: 70px;
        height: 100%;
        position: absolute;
        top: 0;
        background-size: contain;
        cursor: pointer;
        text-align: center;
        -webkit-transition: 0.3s ease-out;
        -o-transition: 0.3s ease-out;
        transition: 0.3s ease-out;
        right: 0;
        font-size: 0;
        color: #414245;
        background-image: linear-gradient(to right, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.3) 100%);
        margin: 0;
    }

    .carousel-default .hero-banner-carousel .owl-nav .owl-next:focus,
    .carousel-default .hero-banner-carousel .owl-nav .owl-prev:focus {
        outline: none;
    }

    .carousel-default .hero-banner-carousel .owl-nav .owl-next:after,
    .carousel-default .hero-banner-carousel .owl-nav .owl-prev:after {
        position: absolute;
        width: 0;
        content: '';
        height: 0;
        top: 48%;
        right: 32px;
        border-style: solid;
        border-color: inherit;
        border-width: 0 2px 2px 0;
        display: inline-block;
        padding: 10px;
        transform: rotate(-45deg);
    }

    .carousel-default .hero-banner-carousel .owl-nav .owl-prev {
        left: 0;
        background-image: linear-gradient(to left, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.3) 100%);
    }

    .carousel-default .hero-banner-carousel .owl-nav .owl-prev:after {
        left: 32px;
        right: auto;
        transform: rotate(135deg);
    }

    .carousel-default .hero-banner-carousel .owl-dots {
        text-align: center;
        position: absolute;
        z-index: 1;
        bottom: 5px;
        left: 0;
        right: 0;
    }

    .carousel-default .hero-banner-carousel .owl-dots .owl-dot {
        cursor: pointer;
        -webkit-user-select: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
        width: 26px;
        height: 26px;
        padding: 3px 3px;
        display: inline-block;
    }

    .carousel-default .hero-banner-carousel .owl-dots .owl-dot.active {
        cursor: default;
    }

    .carousel-default .hero-banner-carousel .owl-dots .owl-dot.active span {
        background: #ffffff;
    }

    .carousel-default .hero-banner-carousel .owl-dots .owl-dot span {
        width: 12px;
        display: block;
        height: 12px;
        border-radius: 50%;
        background: #ABABAB;
    }

    .carousel-default .hero-banner-carousel .hero-banner {
        background-attachment: inherit;
        height: 360px;
    }

    .carousel-default .hero-banner-carousel .owl-stage-outer {
        overflow: hidden;
    }

    .carousel-default .hero-banner-carousel .page-section {
        margin: 20px 0 0;
        height: 100%;
        display: flex;
        align-items: center;
        flex-wrap: wrap;
    }

    .carousel-default .hero-banner-carousel .page-section .link-button {
        margin-bottom: auto;
        color: inherit;
    }

    .carousel-default .hero-banner-carousel .animated {
        animation-duration: 1000ms;
        animation-fill-mode: both;
    }

    .carousel-default .hero-banner-carousel .wiley-slogan {
        width: 100%;
        padding-top: 0;
    }

    .carousel-default .hero-banner-carousel .wiley-slogan p {
        margin-bottom: 10px;
    }

    .carousel-default .hero-banner-carousel .simple-responsive-banner-component {
        position: absolute;
        max-height: 100%;
        overflow: hidden;
    }

    .carousel-default .hero-banner-carousel .simple-responsive-banner-component img {
        width: auto;
        height: 360px;
        max-width: none;
    }

    .carousel-default .hero-banner-carousel .container {
        position: relative;
        height: 360px;
    }

    .carousel-default .hero-banner-carousel .owl-item {
        float: left;
        height: 360px;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .carousel-default .hero-banner-carousel .item {
        height: 360px;
        position: relative;
    }

    .carousel-default .hero-banner-carousel .item .link-item {
        cursor: pointer;
    }

    .carousel-default .hero-banner-carousel:hover .owl-nav .owl-next,
    .carousel-default .hero-banner-carousel:hover .owl-nav .owl-prev {
        color: white;
    }


    .hero-banner {
        position: relative;
        overflow: hidden;
        min-height: 360px;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .hero-banner .simple-responsive-banner-component {
        margin: 0;
        min-height: 0;
    }

    .hero-banner .container {
        position: relative;
    }

    .hero-banner .section-description {
        margin: 0;
    }

    .hero-banner p {
        margin-bottom: 50px;
    }

    .wiley-slogan h1 {
        color: white;
        font-family: 'Source Serif Pro', serif;
        line-height: 63px;
        font-size: 50px;
        font-weight: 600;
        margin: 0;
    }

    .wiley-slogan p {
        color: white;
        font-size: 24px;
        line-height: 30px;
    }

    .wiley-slogan p:first-of-type {
        margin-bottom: 10px;
    }

    .wiley-slogan p:last-of-type {
        margin-bottom: 50px;
    }

    .wiley-slogan .link-button {
        margin-bottom: 45px;
    }

</style>