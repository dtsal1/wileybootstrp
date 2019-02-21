<template>
    <footer class="main-footer-container">
        <div class="container">
            <div class="main-footer-links-container">
                <div class="main-footer-links">
                    <div class="footer-links-title">о компании</div>

                    <ul class="footer-links-items">
                        <!--<li class="yCmsComponent">-->
                        <!--<a href="https://www.wiley.com/en-ru/corporatecitizenship" title="Corporate Citizenship">Corporate Citizenship</a>-->
                        <!--</li>-->
                        <!--<li class="yCmsComponent">-->
                        <!--<a href="https://www.wiley.com/en-ru/corporategovernance" title="Corporate Governance">Corporate Governance</a>-->
                        <!--</li>-->
                    </ul>
                    <!--<ul class="footer-links-items">-->
                        <!--<li class="yCmsComponent">-->
                            <!--<a href="https://www.wiley.com/en-ru/investors" title="Investors">Investors</a>-->
                        <!--</li>-->
                        <!--<li class="yCmsComponent">-->
                        <!--<a href="https://www.wiley.com/en-ru/leadership-team" title="Leadership Team">Leadership Team</a>-->
                        <!--</li>-->
                        <!--<li class="yCmsComponent">-->
                        <!--<a href="https://newsroom.wiley.com/" title="Newsroom">Newsroom</a>-->
                        <!--</li>-->
                        <!--<li class="yCmsComponent">-->
                        <!--<a href="https://www.wiley.com/WileyCDA/Section/id-390059.html" title="The Wiley Foundation">The Wiley Foundation</a>-->
                        <!--</li>-->
                    <!--</ul>-->
                </div>
                <div class="main-footer-links">
                    <div class="footer-links-title">продукты</div>

                </div>
                <div class="main-footer-links">
                    <div class="footer-links-title">карьера в россии</div>
                </div>
                <div class="main-footer-links">
                    <div class="footer-links-title">контакты</div>
                </div>
            </div>
            <div class="footer-social-links">
                <div class="content cke-content"></div></div>
            <div class="main-footer-copyright">
                <div class="footer-copyright-text">
                    <div class="content cke-content"><p><a href="https://www.wiley.com/copyright"><b>Copyright © 2000-2019</b></a> by <a href="https://www.wiley.com/"><b>John Wiley &amp; Sons, Inc.</b></a>, or related companies. All rights reserved.</p></div></div>
                <div class="footer-logo">
                    <div class="simple-banner-component">
                        <a href="https://www.wiley.com/" title="Wiley">
                            <img alt="Wiley" src="../assets/wiley-logo_optimized.png"></a>
                    </div></div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: "wileyFooter"
    }
</script>

<style scoped>

    .main-footer-container {
        font-size: 10px;
        color: #ffffff;
        background-color: rgba(0, 0, 0, 0.87);
    }

    .main-footer-container > .container {
        padding-top: 20px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .main-footer-container > .container:before,
    .main-footer-container > .container:after {
        display: none;
    }

    .main-footer-container .main-footer-links-container {
        display: flex;
        align-items: baseline;
        margin-bottom: 10px;
    }

    .main-footer-container .main-footer-links {
        padding-right: 65px;
    }

    .main-footer-container .footer-links-title {
        margin-bottom: 12px;
        font-size: 11px;
        letter-spacing: 0.24px;
        line-height: 19px;
        font-weight: 500;
        text-transform: lowercase;
        white-space: nowrap;
    }

    .main-footer-container ul.footer-links-items {
        margin: 0;
        padding: 0;
        font-size: 1.1em;
        line-height: 1.6;
        float: left;
        list-style: none;
        margin-right: 30px;
    }

    .main-footer-container ul.footer-links-items li {
        padding-bottom: 5px;
        font-size: 11px;
        line-height: 16px;
        font-weight: 600;
        letter-spacing: normal;
    }

    .main-footer-container ul.footer-links-items li a {
        color: #ffffff;
    }

    .main-footer-container .main-footer-copyright {
        width: 100%;
        padding: 17px 20px 18px 0;
        border-top: 1px solid #424242;
        display: flex;
        align-items: center;
    }

    .main-footer-container .footer-copyright-text {
        font-size: 10px;
        letter-spacing: 0.17px;
        color: #9B9B9B;
    }

    .main-footer-container .footer-copyright-text p {
        margin-bottom: 0;
        font-size: inherit;
    }

    .main-footer-container .footer-copyright-text p a {
        color: #9B9B9B;
    }

    .main-footer-container .footer-logo {
        display: inline-block;
        margin-left: auto;
        width: 96px;
        height: 20px;
        background-size: contain;
        background-repeat: no-repeat;
    }

    .main-footer-container .footer-social-links {
        text-align: center;
    }

    .main-footer-container .footer-social-links a {
        margin: 0 10px 15px;
    }

    .main-footer-container .footer-social-links > a {
        display: inline-block;
        min-width: 20px;
        min-height: 20px;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
    }

    .main-footer-container .footer-social-links > a.fb {
        background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAAhCAMAAADj/gtmAAAANlBMVEUAAAD////////////////////////////////////////////////////////////////////xY8b8AAAAEXRSTlMAECAwP2BwgK+wwM/Q3+Dv8O1mNcMAAABbSURBVHja5c9BDoAgDETRqpQqKjD3v6yQiiF0ZeLOv5u3aumJ14Sab7CcuJMmwEjREMNQsATtkNLUU9bVU6A3NLuS0u5qRBlDTBiTT8lLSUcU/dGe+h/aQk10XJxFFLSUej/yAAAAAElFTkSuQmCC);
    }

    .main-footer-container .footer-social-links > a.tw {
        background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACMAAAAcCAMAAADcK/YTAAAAVFBMVEUAAAD///////////////////////////////////////////////////////////////////////////////////////////////////////////8wXzyWAAAAG3RSTlMAECAwP0BQX2BvcH+Aj5CfoK+wv8DP0N/g7/CN3MwKAAAA00lEQVR4AYXR3XKDIBiE4QWCIUo1/ot7//dZHUrjN6J5Dp3XWQXkFG1gaCx2Oj6BpHpGP4BpOmwsnUxGJvPMVWHjKSPPg8XofeZN8oWPwINxXk16r9UpsRTiRsldqJScSlvYKUaheWDjeDScPjL01fOVazQ6XvKx4diGb03HGzY2jjcUooGXJvxRE6+USFR9NxWpx3Nkzhv/1MKsVeOjuDucxOV/SiqW+6XIlrNMDE50/y0xDYVJJK6qqtPF1wqCX0lpMDhx3XGl1sgzzvuu9t7mgl/2KTq48Xv4HAAAAABJRU5ErkJggg==);
    }

    .main-footer-container .footer-social-links > a.go {
        background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACcAAAAhCAMAAABtJEIaAAAAVFBMVEUAAAD///////////////////////////////////////////////////////////////////////////////////////////////////////////8wXzyWAAAAG3RSTlMAECAwP0BPUF9gb3B/gJCfoK+wv8DP0N/g7/Bjas6/AAABE0lEQVR4AY3Q4W6DIBRA4YuMOqdQNxGR8/7vubV2zY2BpucXhi9wUR71141nozyKeNHZjdnPBSB4b6XhBsptz8zAfqia65833aFpOLPD/14GxoYbIaqjiQ0X9VaBve02/YGI41R8bBnlUsMFYFAuiNh4VMjHIoiIQ12cKd15Pj1TOJYOBmk5k4Cv+2rV7OzERGC5fHxuxUrT3bIhJtR7zk43Au4NF4DvN8/TF7cyBWB6bS7TNC3curaVWyAF7+f8CpoFolUz9lVmVz29zbBWXYJZfXYFjNT/RicqD65+HKKzdUfF2YrL5wcOZKkUgFUPHhlrziQ0NFdmqWYisE/3mdy0KXZuSDxLvbyoG3z862e0LfEL+dghK0fZaagAAAAASUVORK5CYII=);
    }

    @media (max-width: 640px) {
        .main-footer-container > .container {
            padding-top: 30px;
            padding-left: 0;
            padding-right: 0;
        }

        .main-footer-container .main-footer-links-container {
            display: none;
        }

        .main-footer-container .footer-social-links {
            width: 100%;
            padding: 0 10px 15px;
            text-align: center;
        }

        .main-footer-container .footer-social-links a {
            margin: 0 5px 10px;
        }

        .main-footer-container .footer-social-links > a {
            margin: 0 10px 10px;
        }

        .main-footer-container .main-footer-copyright {
            padding: 12px 6% 15px;
            text-align: center;
            overflow: hidden;
        }

        .main-footer-container .footer-copyright-text {
            text-align: left;
            margin-right: 30px;
        }

        .main-footer-container .footer-copyright-text b {
            font-weight: normal;
        }

        .main-footer-container .footer-logo {
            width: 77px;
            height: 16px;
            flex-shrink: 0;
        }
    }

    @media (min-width: 641px) {
        .main-footer-container .footer-social-links {
            margin-right: 20px;
        }

        .main-footer-container .footer-social-links a:first-child {
            margin-left: 0;
        }

        .main-footer-container .footer-social-links a:last-child {
            margin-right: 0;
        }

        .main-footer-container .footer-copyright-text {
            float: left;
        }

        .main-footer-container .footer-copyright-text b {
            font-weight: 400;
        }
    }

    /*.yCmsComponent {*/
        /*position: relative;*/
        /*padding-left: 52px;*/
        /*color: #ffffff;*/
        /*background-color: #5d5d5d;*/
    /*}*/

    /*.yCmsComponent{*/
        /*content: " ";*/
        /*display: block;*/
        /*position: absolute;*/
        /*top: 50%;*/
        /*left: 15px;*/
        /*margin-top: -11px;*/
        /*width: 22px;*/
        /*height: 22px;*/
    /*}*/

</style>