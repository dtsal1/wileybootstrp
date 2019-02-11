<template>
    <header id="main-header-container" class="main-header-container">
        <div class="main-sticky-header affix-top">
            <div class="main-header-navigation">
                <div class="main-navigation-mobile-header">
                    <div class="wileyLogo">
                        <div class="simple-responsive-banner-component">
                            <a href="https://www.wiley.com/en-gb/">
                                <img class="js-responsive-image" alt="Wiley" title="Wiley" style="" src="../assets/b2c-site-logo_desktop_optimized.png">
                            </a>
                        </div>
                    </div>
                    <span type="button" id="openMenu" @click="menuClick" class="navbar_toggle collapsed visible-xs-inline-block">
                             <!--<span class="patty"></span>-->
                          </span>
                    <span class="main-navigation-search-icon icon-search-black visible-xs-inline-block"></span>

                </div>
                <nav id="main-header-navbar" role="navigation" class="collapse navbar-collapse navbar">
                    <ul id="navigation-menu" class="navigation-menu">
                        <li class=""><a href="" class="">{{msgProducts}}</a>
                        </li>
                        <li class=""><a href="" class="">{{msgWork}}</a>
                        </li>
                        <li class=""><a href="" class="">{{msgCompany}}</a>
                        </li>
                        <li class=""><a href="" class="">{{msgContact}}</a>
                        </li>

                    </ul>
                </nav>
            </div>
            <app-search></app-search>
           </div>
    </header>
</template>

<script>
    import search from "./search.vue"
    export default {
        name: "wileyHeader",
        data() {
            return {
                msgProducts: "продукты",
                msgWork: "работа в россии",
                msgCompany: "о компании",
                msgContact: "связаться с нами"
            }
        },
        components: {
            appSearch: search
        },
        methods:{
            menuClick (e) {
                e.preventDefault();

            }

        }


    }
</script>

<style scoped>

    @font-face {
        font-family: 'Material Icons';
        font-style: normal;
        font-weight: 400;
        src: url(https://fonts.gstatic.com/s/materialicons/v43/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2) format('woff2');
    }

    .material-icons {
        font-family: 'Material Icons';
        font-weight: normal;
        font-style: normal;
        font-size: 24px;
        line-height: 1;
        letter-spacing: normal;
        text-transform: none;
        display: inline-block;
        white-space: nowrap;
        word-wrap: normal;
        direction: ltr;
        -webkit-font-feature-settings: 'liga';
        -webkit-font-smoothing: antialiased;
    }
    @media (min-width: 641px) {
        .main-header-container .simple-responsive-banner-component {
            margin: 0;
        }

        .main-header-container .affix {
            width: 100%;
        }

        .main-navigation-mobile-header {
            margin-right: 40px;
        }

        .main-header-navigation {
            position: relative;
            margin: 0;
            min-width: 1260px;
            z-index: 1000;
            border-bottom: 1px solid #979797;
            transition: all .3s linear;
            background-color: white;
            top: 0;
            height: 60px;
            box-sizing: border-box;
            display: flex;
            align-items: center;
            width: 100%;
            padding-left: 20px;
            padding-right: 30px;
        }

        .main-header-navigation .navbar-collapse {
            display: flex !important;
            margin: 0;
            min-height: 0;
            border: none;
            position: static;
            flex: 1;
            padding: 0;
            justify-content: space-between;
        }

        .main-header-navigation .navbar-collapse:before {
            display: none;
        }

        .main-header-navigation .wileyLogo img {
            width: 105px;
            max-width: 105px;
        }
    }
    @media (min-width: 641px) {
        .navigation-menu{
            margin: 0;
            padding: 0;
            list-style: none;
            display: flex;
            font-family: 'Open Sans', sans-serif;
            flex: 1;
            text-transform: uppercase;
            font-size: 1.6em;
        }

        .navigation-menu > li {
            display: inline-block;
            line-height: 60px;
            padding-right: 20px;
        }

        .navigation-menu > li.dropdown-submenu {
            position: relative;
        }

        .navigation-menu > li.dropdown-submenu:after {
            position: absolute;
            content: '';
            right: 5px;
            display: inline-block;
            width: 0;
            height: 0;
            top: 26px;
            border: none;
            border-width: 0 1px 1px 0;
            padding: 3px;
            transform: rotate(90deg);
        }

        .navigation-menu> li.dropdown-submenu.hover:after {
            top: 29px;
            transform: rotate(-135deg);
        }

        .navigation-menu > li:last-child a {
            padding-right: 0;
        }

        .navigation-menu > li > a {
            padding: 0 20px;
            color: #414245;
            font-weight: 600;
            height: 100%;
            box-sizing: border-box;
            top: 1px;
            display: block;
            letter-spacing: 0.27px;
            white-space: nowrap;
        }

        .navigation-menu > li > a:hover,
        .navigation-menu > li > a:focus {
            text-decoration: none;
            outline: 0 solid transparent;
            color: #009ca9;
        }

        .navigation-menu > li > a.collapsed {
            position: relative;
            padding-right: 0;
        }

        .navigation-menu > li.hover .dropdown-menu {
            display: block;
            z-index: 1;
        }

        .navigation-menu > li.hover > a {
            color: #009ca9;
        }

        .navigation-menu> li:hover > a,
        .navigation-menu > li:focus > a {
            color: #009ca9;
        }
        dropdown-menu {
            font-family: 'Open Sans', sans-serif;
            border: none;
            position: absolute;
            z-index: -1;
            float: none;
            top: 100%;
            max-width: 1240px;
            min-width: 900px;
            max-height: 80vh;
            overflow: hidden;
            box-sizing: border-box;
            -webkit-overflow-scrolling: touch;
            left: 0;
            padding-top: 0;
            right: 0;
            margin: auto;
            display: none;
            background-color: #ffffff;
        }

        .dropdown-menu.collapse.in {
            display: block;
            z-index: 1;
            right: auto;
        }

        .dropdown-menu .dropdown-item-title {
            display: none;
        }

        .dropdown-menu .toggle-dropdown {
            left: 0;
            position: relative;
            top: 0;
            bottom: 0;
            width: 30px;
            height: 20px;
            padding: 0 20px;
            box-sizing: border-box;
        }

        .dropdown-menu .toggle-dropdown:after {
            position: absolute;
            width: 0;
            content: '';
            height: 0;
            top: 13px;
            right: 20px;
            border: solid #c2c3c6;
            border-width: 0 1px 1px 0;
            display: inline-block;
            padding: 3px;
            transform: rotate(-45deg);
            -webkit-transform: rotate(-45deg);
        }
    }
    @media (max-width: 846px) {
        .navigation-menu{
            margin: 0;
            padding: 0;
            list-style: none;
            display: flex;
            font-family: 'Open Sans', sans-serif;
            flex: 1;
            text-transform: uppercase;
            font-size: 1.3em;
        }

        .navigation-menu> li {
            display: inline-block;
            line-height: 60px;
            padding-right: 2px;
        }

        .navigation-menu> li.dropdown-submenu {
            position: relative;
        }

        .navigation-menu> li.dropdown-submenu:after {
            position: absolute;
            content: '';
            right: 5px;
            display: inline-block;
            width: 0;
            height: 0;
            top: 26px;
            border: none;
            border-width: 0 1px 1px 0;
            padding: 3px;
            transform: rotate(90deg);
        }

        .navigation-menu > li.dropdown-submenu.hover:after {
            top: 29px;
            transform: rotate(-135deg);
        }

        .navigation-menu > li:last-child a {
            padding-right: 0;
        }

        .navigation-menu > li > a {
            padding: 0 20px;
            color: #414245;
            font-weight: 600;
            height: 100%;
            box-sizing: border-box;
            top: 1px;
            display: block;
            letter-spacing: 0.27px;
            white-space: nowrap;
        }

        .navigation-menu > li > a:hover,
        .navigation-menu> li > a:focus {
            text-decoration: none;
            outline: 0 solid transparent;
            color: #009ca9;
        }

        .navigation-menu > li > a.collapsed {
            position: relative;
            padding-right: 0;
        }

        .navigation-menu > li.hover .dropdown-menu {
            display: block;
            z-index: 1;
        }

        .navigation-menu > li.hover > a {
            color: #009ca9;
        }

        .navigation-menu > li:hover > a,
        .navigation-menu > li:focus > a {
            color: #009ca9;
        }

    }
    @media (max-width: 640px) {
        .main-header-container {
            margin: 0;
            height: 60px;
        }

        .main-header-container .main-sticky-header {
            height: 60px;
            box-shadow: 0px 8px 8px -7px rgba(0, 0, 0, 0.19);
        }

        .main-header-container .main-sticky-header.no-shadow,
        .main-header-container .main-sticky-header.no-shadow.affix {
            box-shadow: none;
        }

        .main-header-container .main-header-navigation {
            width: 100%;
            overflow: hidden;
            transition: all 0.2s linear;
            background: white;
            box-sizing: border-box;
            z-index: 10;
            position: relative;
        }

        .main-header-container .main-header-navigation.collapse.in {
            height: calc(100vh - 60px);
            height: calc(var(--vh, 1vh) * 100 - 60px);
        }

        .main-header-container .main-navigation-search {
            position: fixed;
            top: -100px;
            width: 100%;
            height: 52px;
            padding: 0;
            box-sizing: border-box;
            transition: all 0.5s ease-out;
            -webkit-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
            -moz-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
            box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
        }

        .main-header-container .main-navigation-search.open {
            top: 60px;
        }

        .main-header-container .main-navigation-search > .container {
            padding: 0;
        }

        .main-header-container .main-navigation-search > .container:after,
        .main-header-container .main-navigation-search > .container:before {
            display: none;
        }

        .main-header-container .main-navigation-search .input-group {
            background-color: #efeff0;
        }

        .main-header-container .main-navigation-search .input-group .input-group-btn button {
            height: 52px;
            width: 40px;
            padding-right: 20px;
            background-color: unset;
            font-style: normal;
            font-weight: normal;
            background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjIycHgiIHZpZXdCb3g9IjAgMCAyMiAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT45RjI3MjYzQy0yRjhCLTRCQjQtODJDNS02MDY4OTNGRENCNUI8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9IkZpbmFsLVZpc3VhbC1EZXNpZ25zIiBzdHJva2U9Im5vbmUiIHN0cm9rZS13aWR0aD0iMSIgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj4gICAgICAgIDxnIGlkPSJBLU1vYmlsZS1TUlAtZnVsbC1zY3JlZW4iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0yMjQuMDAwMDAwLCAtMTkuMDAwMDAwKSIgZmlsbD0iIzAwMDAwMCIgZmlsbC1ydWxlPSJub256ZXJvIj4gICAgICAgICAgICA8ZyBpZD0iR3JvdXAtMTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIyMy4wMDAwMDAsIDE4LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0ic2VhcmNoLWNvcHkiPiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIyLjQ5NDMyNjksMjEuNzA0MjM1MyBMMTUuMTQ5MTY2OSwxNC4zNTkwODUzIEMxNy45OTYzNTgzLDExLjA4Njk4NzUgMTcuNzQ1Njk4MSw2LjE0OTAwNDczIDE0LjU4MTgwMTQsMy4xODIwMzk4MiBDMTEuNDE3OTA0NywwLjIxNTA3NDkwOCA2LjQ3NDAxNDc4LDAuMjgxODM0MDg4IDMuMzkxMzg1MTUsMy4zMzMxNDgxNiBDMC4zMDg3NTU1MjEsNi4zODQ0NjIyNCAwLjE5MTUyMTE2MiwxMS4zMjc0MTI4IDMuMTI2MDI3MDQsMTQuNTIxNDM4MiBDNi4wNjA1MzI5MiwxNy43MTU0NjM2IDEwLjk5NTY5OSwxOC4wMTY1MjkyIDE0LjI5NjY5NjksMTUuMjAyODk1MyBMMjEuNjQ2Njk2OSwyMi41NTI4OTUzIEMyMS44ODExNTIzLDIyLjc4NjMwOSAyMi4yNjAzMzksMjIuNzg1Nzc4NCAyMi40OTQxNDA0LDIyLjU1MTcwOTYgQzIyLjcyNzk0MTcsMjIuMzE3NjQwNyAyMi43MjgwMzg2LDIxLjkzODQ1MzYgMjIuNDk0MzU2OSwyMS43MDQyNjUzIEwyMi40OTQzMjY5LDIxLjcwNDIzNTMgWiBNMi4xNjQyNDY5MSw5LjAyOTkxNTI5IEMyLjE2NDA1Mjc2LDYuMjM4OTI0MzggMy44NDUxNTU3MiwzLjcyMjY0NDQ4IDYuNDIzNjM5MzYsMi42NTQ0NDM5OCBDOS4wMDIxMjMwMSwxLjU4NjI0MzQ3IDExLjk3MDE4MjUsMi4xNzY0OTMwNiAxMy45NDM3Nzk3LDQuMTQ5OTUzMDIgQzE1LjkxNzM3Nyw2LjEyMzQxMjk3IDE2LjUwNzgzMyw5LjA5MTQzMTM5IDE1LjQzOTgxMTksMTEuNjY5OTg5MyBDMTQuMzcxNzkwOCwxNC4yNDg1NDczIDExLjg1NTYyNzgsMTUuOTI5ODI1MyA5LjA2NDYzNjkxLDE1LjkyOTgyNTMgQzUuMjU1NTgyNDcsMTUuOTI1NjMxOCAyLjE2ODcwNTQxLDEyLjgzODk2OTQgMi4xNjQyNDY5MSw5LjAyOTkxNTI5IFoiIGlkPSJTaGFwZSI+PC9wYXRoPiAgICAgICAgICAgICAgICA8L2c+ICAgICAgICAgICAgPC9nPiAgICAgICAgPC9nPiAgICA8L2c+PC9zdmc+);
        }

        .main-header-container .main-navigation-search .input-group .input-group-btn button:before {
            top: 0;
            bottom: 0;
            margin: auto;
        }

        .main-header-container .main-navigation-search .input-group .input-group-btn button:focus {
            background-color: unset;
        }

        .main-header-container .main-navigation-search .input-group .main-navigation-search-input {
            height: 52px;
            padding: 0 15px;
            font-size: 1.3em;
            font-weight: 600;
            color: #000000;
            border: none;
        }

        .main-header-container .main-navigation-search .input-group .main-navigation-search-input::placeholder {
            color: #979797;
        }

        .main-header-container .main-navigation-search .input-group .main-navigation-search-input:focus + .input-group-btn button {
            background-color: unset;
        }

        .main-header-container .main-navigation-search-autocomplete {
            max-height: calc(100vh - 212px);
            max-height: calc(var(--vh, 1vh) * 100 - 212px);
            margin-top: 0;
            padding: 15px 15px 5px;
            border: 1px solid #dddedf;
            border-left: none;
            border-right: none;
            -webkit-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
            -moz-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
            box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section {
            padding-bottom: 20px;
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a {
            font-weight: 700;
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a b {
            color: rgba(0, 0, 0, 0.87);
            font-weight: 400;
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item,
        .main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item {
            line-height: 2.2;
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section h3 {
            margin-bottom: 5px;
        }

        .main-header-container .main-navigation-search-autocomplete .searchresults-section .all-results-link {
            font-weight: 600;
            color: #1AA6B1;
            text-decoration: none;
        }

        .main-header-container .main-navigation-mobile-header {
            z-index: 2;
            height: 60px;
            position: relative;
            padding: 0 0 0 20px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
            background: white;
            border-bottom: 1px solid #dddedf;
        }

        .main-header-container .main-navigation-mobile-header .my-cart-link {
            margin: 0 20px 0 20px;
        }

        .main-header-container .main-navigation-mobile-header .wileyLogo {
            margin-right: auto;
        }

        .main-header-container .main-navigation-mobile-header .wileyLogo .simple-responsive-banner-component {
            margin: 0;
        }

        .main-header-container .main-navigation-mobile-header .wileyLogo a,
        .main-header-container .main-navigation-mobile-header .wileyLogo img {
            width: 90px;
            height: 20px;
        }

        .main-header-container .navigation-links-items {
            margin: 0;
            padding: 0;
            position: static;
            display: block;
        }

        .main-header-container .navigation-links-items .navigation-link-item {
            margin-left: 15px;
            padding: 10px 0;
        }

        .main-header-container .navigation-links-items .navigation-link-item:first-child {
            margin-left: 15px;
        }

        .main-header-container .navigation-links-items .navigation-link-item.my-account-link {
            position: absolute;
            right: 20px;
            bottom: 10px;
            top: unset;
            line-height: 44px;
            padding-bottom: 0;
            margin: 0;
            font-size: 16px;
        }

        .main-header-container .navigation-links-items .navigation-link-item.my-account-link:before {
            content: "";
            width: 17px;
            height: 19px;
            margin-right: 5px;
            background-size: contain;
            background-repeat: no-repeat;
            vertical-align: middle;
            display: inline-block;
            background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyNHB4IiBoZWlnaHQ9IjI0cHgiIHZpZXdCb3g9IjAgMCAyNCAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT5NeSBhY2NvdW50PC90aXRsZT4gICAgPGRlc2M+Q3JlYXRlZCB3aXRoIFNrZXRjaC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9Ik15LWFjY291bnQiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiPiAgICAgICAgPGcgaWQ9Ikdyb3VwLTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDYuMDAwMDAwLCAzLjAwMDAwMCkiIGZpbGwtcnVsZT0ibm9uemVybyIgc3Ryb2tlPSIjMDAwMDAwIj4gICAgICAgICAgICA8Y2lyY2xlIGlkPSJPdmFsIiBjeD0iNiIgY3k9IjYiIHI9IjYiPjwvY2lyY2xlPiAgICAgICAgPC9nPiAgICAgICAgPHBhdGggZD0iTTguNjQyNDU2MDUsMTQuMjg0MTc5NyBDNS4xNTc3NTU1MywxOC4xMTAwNjM1IDMuNDE1NDA1MjcsMjAuODIxMzI2NSAzLjQxNTQwNTI3LDIyLjQxNzk2ODcgQzcuMDk4MjY2NiwyMi40MTc5Njg3IDE2LjcwOTU5NDcsMjIuNDE3OTY4NyAyMC41NzU1NjE1LDIyLjQxNzk2ODcgQzIwLjU3NTU2MTUsMjAuODYxMzYwMiAxOC43ODM4OTQ5LDE4LjE1MDA5NzIgMTUuMjAwNTYxNSwxNC4yODQxNzk3IiBpZD0iTGluZS00IiBzdHJva2U9IiMwMDAwMDAiIHN0cm9rZS1saW5lY2FwPSJzcXVhcmUiPjwvcGF0aD4gICAgPC9nPjwvc3ZnPg==);
        }

        .main-header-container .navbar-collapse {
            margin: 0;
            padding: 0;
            border-top: none;
            width: 100%;
            height: calc(100vh - 60px);
            height: calc(var(--vh, 1vh) * 100 - 60px) !important;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
            background: white;
        }

        .main-header-container .navbar-collapse:before {
            display: none;
        }

        .main-header-container .main-navigation-search-icon {
            -webkit-box-sizing: content-box;
            -moz-box-sizing: content-box;
            box-sizing: content-box;
            font-size: 2em;
            width: 42px;
            height: 60px;
            line-height: 60px;
            color: #000000;
            border-left: 1px solid transparent;
            border-right: 1px solid transparent;
        }

        .main-header-container .main-navigation-search-icon:after,
        .main-header-container .main-navigation-search-icon:before {
            right: 0;
            margin: auto;
            bottom: 0;
            left: 0;
            top: 0;
        }

        .main-header-container .main-navigation-search-icon.active {
            border-left: 1px solid #c2c3c6;
            border-right: 1px solid #c2c3c6;
            background-color: #efeff0;
        }

        .main-header-container .main-navigation-search-icon.active:after,
        .main-header-container .main-navigation-search-icon.active:before {
            position: absolute;
            z-index: 1;
            display: block;
            width: 24px;
            height: 1px;
            border-radius: 2px;
            background: #000000;
            content: '';
        }

        .main-header-container .main-navigation-search-icon.active:after {
            -webkit-transform: rotate(45deg);
            -ms-transform: rotate(45deg);
            -o-transform: rotate(45deg);
            transform: rotate(45deg);
        }

        .main-header-container .main-navigation-search-icon.active:before {
            -webkit-transform: rotate(-45deg);
            -ms-transform: rotate(-45deg);
            -o-transform: rotate(-45deg);
            transform: rotate(-45deg);
        }

        .main-header-container .navbar_toggle {
            margin: 0;
            order: 1;
            height: 60px;
            line-height: 60px;
            border-left: 1px solid #dddedf;
            background-color: white;
            padding: 0 10px;
            box-sizing: border-box;
            top: 1px;
        }

        .main-header-container .navbar_toggle.collapsed {
            border-color: transparent;
            height: 59px;
            top: 0;
        }

        .main-header-container .navbar_toggle .patty {
            -webkit-transition: all 0.2s ease;
            -o-transition: all 0.2s ease;
            transition: all 0.2s ease;
            top: -4px;
            position: relative;
            width: 24px;
            height: 1px;
            margin: 0;
            padding: 0;
            border-radius: 2px;
            display: inline-block;
            background: black;
        }

        .main-header-container .navbar_toggle .patty:after,
        .main-header-container .navbar_toggle .patty:before {
            -webkit-transition: all 0.2s ease;
            -o-transition: all 0.2s ease;
            transition: all 0.2s ease;
            position: absolute;
            z-index: 1;
            display: block;
            width: 24px;
            height: 1px;
            border-radius: 2px;
            background: black;
            content: '';
        }

        .main-header-container .navbar_toggle .patty:after {
            top: 6px;
        }

        .main-header-container .navbar_toggle .patty:before {
            top: -6px;
        }

        .main-header-container .navbar_toggle:not(.collapsed) .patty {
            background: none;
        }

        .main-header-container .navbar_toggle:not(.collapsed) .patty:before {
            -webkit-transform: rotate(-45deg);
            -ms-transform: rotate(-45deg);
            -o-transform: rotate(-45deg);
            transform: rotate(-45deg);
            top: 0;
        }

        .main-header-container .navbar_toggle:not(.collapsed) .patty:after {
            -webkit-transform: rotate(45deg);
            -ms-transform: rotate(45deg);
            -o-transform: rotate(45deg);
            transform: rotate(45deg);
            top: 0;
        }
    }
</style>