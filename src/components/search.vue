<template>
    <div class="main-navigation-search">
        <div class="container">
            <form name="search_form_SearchBox" method="get" action="https://www.wiley.com/en-gb/search">
                <div class="input-group">
                    <input type="search" id="js-site-search-input" aria-label="site search" class="form-control main-navigation-search-input js-site-search-input ui-autocomplete-input" name="pq" value="" maxlength="100" placeholder="Enter your search by Title, Author, Keyword or ISBN" data-options="{&quot;autocompleteUrl&quot; : &quot;/en-gb/search/autocomplete/SearchBox&quot;,&quot;minCharactersBeforeRequest&quot; : &quot;3&quot;,&quot;waitTimeBeforeRequest&quot; : &quot;500&quot;,&quot;displayProductImages&quot; : false}" autocomplete="off">
                    <span class="input-group-btn">
                            <button type="submit" class="glyphicon glyphicon-search">Search</button>
                        </span>
                </div>
                <!--<ul id="ui-id-1" tabindex="0" class="ui-menu ui-widget ui-widget-content ui-autocomplete ui-front" style="display: none;">-->

                <!--</ul>-->
            </form>

        </div>
        <!--<div class="box">-->
            <!--<div class="container-2">-->
                <!--<span class="icon"><i class="fa fa-search"></i></span>-->
                <!--<input type="search" id="search" placeholder="Поиск..." />-->
            <!--</div>-->
        <!--</div>-->
    </div>
</template>

<script>
    export default {
        name: "search"
    }
</script>

<style scoped>
    .input-group-addon,
    .input-group-btn,
    .input-group .form-control {
        display: table-cell;
    }
    .input-group {
        position: relative;
        display: table;
        border-collapse: separate;
    }
    .input-group-addon,
    .input-group-btn {
        width: 1%;
        white-space: nowrap;
        vertical-align: middle;
    }

    .main-header-container .main-navigation-search {
        height: 48px;
        padding: 24px 0;
        position: relative;
        z-index: 1;
        box-sizing: content-box;
    }
    .main-header-container .main-navigation-search > .container {
        max-width: 840px;
    }
    .main-header-container .main-navigation-search .input-group {
        width: 100%;
    }
    .main-header-container .main-navigation-search .input-group .main-navigation-search-input {
        width: 100%;
        height: 48px;
        padding: 0 14px;
        font-size: 1.6em;
        background: none;
        box-shadow: none;
        border: 1px solid #c2c3c6;
        border-right: none;
    }

    .main-header-container .main-navigation-search .input-group .main-navigation-search-input::placeholder {
        color: #d8d9da;
    }

    .main-header-container .main-navigation-search .input-group .main-navigation-search-input::-ms-clear {
        display: none;
    }

    .main-header-container .main-navigation-search-autocomplete {
        position: relative;
        max-height: calc(100vh - 125px);
        width: auto !important;
        margin-top: -1px;
        padding: 20px 20px 5px;
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.24px;
        background: white;
        border: 1px solid #979797;
        overflow-y: auto;
    }
    .main-header-container .main-navigation-search .input-group .input-group-btn button {
        width: 48px;
        height: 48px;
        background-color: #414245;
        outline: none;
        cursor: pointer;
        font-size: 0;
        transition: background-color, 0.3s, linear;
        border: none;
        background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjIycHgiIHZpZXdCb3g9IjAgMCAyMiAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT42MDQ5N0NENC1BMEZFLTQwQzctQUU0NC1GMEQzMDZBQkJDMjA8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxnIGlkPSJGaW5hbC1WaXN1YWwtRGVzaWducyIgc3Ryb2tlPSJub25lIiBzdHJva2Utd2lkdGg9IjEiIGZpbGw9Im5vbmUiIGZpbGwtcnVsZT0iZXZlbm9kZCI+ICAgICAgICA8ZyBpZD0iSG9tZS1QYWdlX0Jhbm5lci1BbGlnbmVkLUxlZnQtIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTA5NS4wMDAwMDAsIC05Ny4wMDAwMDApIiBmaWxsPSIjRkZGRkZGIiBmaWxsLXJ1bGU9Im5vbnplcm8iPiAgICAgICAgICAgIDxnIGlkPSJTZWFyY2giIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMxMC4wMDAwMDAsIDg0LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0iSWNvbl9TZWFyY2giIHRyYW5zZm9ybT0idHJhbnNsYXRlKDc4NS4wMDAwMDAsIDEzLjAwMDAwMCkiPiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIxLjQ5NDMyNjksMjAuNzA0MjM1MyBMMTQuMTQ5MTY2OSwxMy4zNTkwODUzIEMxNi45OTYzNTgzLDEwLjA4Njk4NzUgMTYuNzQ1Njk4MSw1LjE0OTAwNDczIDEzLjU4MTgwMTQsMi4xODIwMzk4MiBDMTAuNDE3OTA0NywtMC43ODQ5MjUwOTIgNS40NzQwMTQ3OCwtMC43MTgxNjU5MTIgMi4zOTEzODUxNSwyLjMzMzE0ODE2IEMtMC42OTEyNDQ0NzksNS4zODQ0NjIyNCAtMC44MDg0Nzg4MzgsMTAuMzI3NDEyOCAyLjEyNjAyNzA0LDEzLjUyMTQzODIgQzUuMDYwNTMyOTIsMTYuNzE1NDYzNiA5Ljk5NTY5ODk1LDE3LjAxNjUyOTIgMTMuMjk2Njk2OSwxNC4yMDI4OTUzIEwyMC42NDY2OTY5LDIxLjU1Mjg5NTMgQzIwLjg4MTE1MjMsMjEuNzg2MzA5IDIxLjI2MDMzOSwyMS43ODU3Nzg0IDIxLjQ5NDE0MDQsMjEuNTUxNzA5NiBDMjEuNzI3OTQxNywyMS4zMTc2NDA3IDIxLjcyODAzODYsMjAuOTM4NDUzNiAyMS40OTQzNTY5LDIwLjcwNDI2NTMgTDIxLjQ5NDMyNjksMjAuNzA0MjM1MyBaIE0xLjE2NDI0NjkxLDguMDI5OTE1MjkgQzEuMTY0MDUyNzYsNS4yMzg5MjQzOCAyLjg0NTE1NTcyLDIuNzIyNjQ0NDggNS40MjM2MzkzNiwxLjY1NDQ0Mzk4IEM4LjAwMjEyMzAxLDAuNTg2MjQzNDcgMTAuOTcwMTgyNSwxLjE3NjQ5MzA2IDEyLjk0Mzc3OTcsMy4xNDk5NTMwMiBDMTQuOTE3Mzc3LDUuMTIzNDEyOTcgMTUuNTA3ODMzLDguMDkxNDMxMzkgMTQuNDM5ODExOSwxMC42Njk5ODkzIEMxMy4zNzE3OTA4LDEzLjI0ODU0NzMgMTAuODU1NjI3OCwxNC45Mjk4MjUzIDguMDY0NjM2OTEsMTQuOTI5ODI1MyBDNC4yNTU1ODI0NywxNC45MjU2MzE4IDEuMTY4NzA1NDEsMTEuODM4OTY5NCAxLjE2NDI0NjkxLDguMDI5OTE1MjkgWiIgaWQ9IlNoYXBlIj48L3BhdGg+ICAgICAgICAgICAgICAgIDwvZz4gICAgICAgICAgICA8L2c+ICAgICAgICA8L2c+ICAgIDwvZz48L3N2Zz4=);
        background-repeat: no-repeat;
        background-position: center;
        background-size: 24px;
    }

    .main-header-container .main-navigation-search .input-group-btn button.glyphicon-search {
        top: 0;
    }

    .main-header-container .main-navigation-search .input-group-btn button.glyphicon-search:before {
        display: none;
    }

    @media (max-width:640px) {
        .main-header-container .main-navigation-search .input-group-btn {
            display: table-cell;
        }

        span.input-group-btn button {
            font-size: 0 !important;
        }

        .input-group-btn button.glyphicon-search:before {
            font-size: 26px !important;
        }

        .main-header-container .main-navigation-search .input-group .input-group-btn button {
            padding: 0 0;
            width: 55px;
        }

        .main-header-container .input-group-btn button.glyphicon-search {
            margin-top: -1px;
            border-radius: 3px;
        }

        .main-header-container .main-navigation-search .input-group .main-navigation-search-input {
            border-radius: 3px;
            width: 98%;
            box-shadow: none;
        }

        .main-header-container .main-navigation-search .input-group-btn button.glyphicon-search:before {
            display: block;
        }
    }
    @media (min-width:641px) {

        .input-group-btn button.glyphicon-search {
            font-family: "Open Sans", "sans-serif" !important;
            font-size: 18px;
            line-height: 25px;
        }

    }
    @media (min-width: 641px) {
        .container {
            max-width: 1260px;
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

        /*.main-header-container .main-header-navigation {*/
            /*width: 100%;*/
            /*overflow: hidden;*/
            /*transition: all 0.2s linear;*/
            /*background: white;*/
            /*box-sizing: border-box;*/
            /*z-index: 10;*/
            /*position: relative;*/
        /*}*/

        /*.main-header-container .main-header-navigation.collapse.in {*/
            /*height: calc(100vh - 60px);*/
            /*height: calc(var(--vh, 1vh) * 100 - 60px);*/
        /*}*/

        .main-header-container .main-navigation-search {
            position: fixed;
            top: 60px;
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
            /*border: 1px solid #dddedf;*/
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
            /*border-bottom: 1px solid #dddedf;*/
        }

        .main-header-container .main-navigation-mobile-header .my-cart-link {
            margin: 0 20px 0 20px;
        }

        .main-header-container .main-navigation-mobile-header .logo {
            margin-right: auto;
        }

        .main-header-container .main-navigation-mobile-header .logo .simple-responsive-banner-component {
            margin: 0;
        }

        .main-header-container .main-navigation-mobile-header .logo a,
        .main-header-container .main-navigation-mobile-header .logo img {
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

        .main-header-container .navbar-toggle {
            margin: 0;
            order: 1;
            height: 60px;
            line-height: 60px;
            /*border-left: 1px solid #dddedf;*/
            background-color: white;
            padding: 0 10px;
            box-sizing: border-box;
            top: 1px;
        }

        .main-header-container .navbar-toggle.collapsed {
            border-color: transparent;
            height: 59px;
            top: 0;
        }

        .main-header-container .navbar-toggle .patty {
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

        .main-header-container .navbar-toggle .patty:after,
        .main-header-container .navbar-toggle .patty:before {
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

        .main-header-container .navbar-toggle .patty:after {
            top: 6px;
        }

        .main-header-container .navbar-toggle .patty:before {
            top: -6px;
        }

        .main-header-container .navbar-toggle:not(.collapsed) .patty {
            background: none;
        }

        .main-header-container .navbar-toggle:not(.collapsed) .patty:before {
            -webkit-transform: rotate(-45deg);
            -ms-transform: rotate(-45deg);
            -o-transform: rotate(-45deg);
            transform: rotate(-45deg);
            top: 0;
        }

        .main-header-container .navbar-toggle:not(.collapsed) .patty:after {
            -webkit-transform: rotate(45deg);
            -ms-transform: rotate(45deg);
            -o-transform: rotate(45deg);
            transform: rotate(45deg);
            top: 0;
        }
    }
</style>