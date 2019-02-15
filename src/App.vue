<template>
  <div id="app">

      <app-header></app-header>

  </div>


</template>

<script>
import wileyHeader from "./components/wileyHeader.vue"


export default {
  name: 'app',
  data () {
    return {

    }
  },
    components: {
        appHeader: wileyHeader

    }
}


</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
html {
    font-size: 62.5%;
    min-height: 100% !important;
    height: 100%;
}

html.has-drawer {
    overflow: hidden;
    height: 100%;
    position: fixed;
    width: 100%;
}

body {
    background: #ffffff;
    font-family: 'Open Sans', sans-serif;
    font-size: inherit;
    line-height: 1.4;
    color: #000000;
    overflow-x: auto;
    min-height: 100%;
}

body.has-drawer {
    overflow: hidden;
    height: 100%;
    width: 100%;
    position: fixed;
}

/*.input-group {*/
    /*position: relative;*/
    /*display: table;*/
    /*border-collapse: separate;*/
/*}*/


/*.input-group-addon,*/
/*.input-group-btn,*/
/*.input-group .form-control {*/
    /*display: table-cell;*/
/*}*/

/*.input-group-addon,*/
/*.input-group-btn {*/
    /*width: 1%;*/
    /*white-space: nowrap;*/
    /*vertical-align: middle;*/
/*}*/

.navbar {
    position: relative;
    min-height: 50px;
    margin-bottom: 20px;
    border: 1px solid transparent;
}

@media (min-width: 641px) {
    .navbar {
        border-radius: 0;
    }
}

@media (min-width: 641px) {
    .navbar-header {
        float: left;
    }
}

.navbar-collapse {
    overflow-x: visible;
    padding-right: 10px;
    padding-left: 10px;
    border-top: 1px solid transparent;
    box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
    -webkit-overflow-scrolling: touch;
}

.navbar-collapse.in {
    overflow-y: auto;
}

@media (min-width: 641px) {
    .navbar-collapse {
        width: auto;
        border-top: 0;
        box-shadow: none;
    }

    .navbar-collapse.collapse {
        display: block !important;
        height: auto !important;
        padding-bottom: 0;
        overflow: visible !important;
    }

    .navbar-collapse.in {
        overflow-y: visible;
    }

    .navbar-fixed-top .navbar-collapse,
    .navbar-static-top .navbar-collapse,
    .navbar-fixed-bottom .navbar-collapse {
        padding-left: 0;
        padding-right: 0;
    }
}

.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
    max-height: 340px;
}

@media (max-width: 320px) and (orientation: landscape) {
    .navbar-fixed-top .navbar-collapse,
    .navbar-fixed-bottom .navbar-collapse {
        max-height: 200px;
    }
}

.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
    margin-right: -10px;
    margin-left: -10px;
}

@media (min-width: 641px) {
    .container > .navbar-header,
    .container-fluid > .navbar-header,
    .container > .navbar-collapse,
    .container-fluid > .navbar-collapse {
        margin-right: 0;
        margin-left: 0;
    }
}

.navbar-static-top {
    z-index: 1000;
    border-width: 0 0 1px;
}

@media (min-width: 641px) {
    .navbar-static-top {
        border-radius: 0;
    }
}

.navbar-fixed-top,
.navbar-fixed-bottom {
    position: fixed;
    right: 0;
    left: 0;
    z-index: 1030;
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
}

@media (min-width: 641px) {
    .navbar-fixed-top,
    .navbar-fixed-bottom {
        border-radius: 0;
    }
}

.navbar-fixed-top {
    top: 0;
    border-width: 0 0 1px;
}

.navbar-fixed-bottom {
    bottom: 0;
    margin-bottom: 0;
    border-width: 1px 0 0;
}

.navbar-brand {
    float: left;
    padding: 15px 10px;
    font-size: 18px;
    line-height: 20px;
    height: 50px;
}

.navbar-brand:hover,
.navbar-brand:focus {
    text-decoration: none;
}

@media (min-width: 641px) {
    .navbar > .container .navbar-brand,
    .navbar > .container-fluid .navbar-brand {
        margin-left: -10px;
    }
}

.navbar-toggle {
    position: relative;
    float: right;
    margin-right: 10px;
    padding: 9px 10px;
    margin-top: 8px;
    margin-bottom: 8px;
    background-color: transparent;
    background-image: none;
    border: 1px solid transparent;
    outline: none;
    border-radius: 0;
}

.navbar-toggle:focus {
    outline: 0;
}

.navbar-toggle .icon-bar {
    display: block;
    width: 22px;
    height: 2px;
    border-radius: 1px;
}

.navbar-toggle .icon-bar + .icon-bar {
    margin-top: 4px;
}

@media (min-width: 641px) {
    .navbar-toggle {
        display: none;
    }
}

.navbar-nav {
    margin: 7.5px -10px;
}

.navbar-nav > li > a {
    padding-top: 10px;
    padding-bottom: 10px;
    line-height: 20px;
}

/*@media (max-width: 640px) {*/
    /*.navbar-nav .open .dropdown-menu {*/
        /*position: static;*/
        /*float: none;*/
        /*width: auto;*/
        /*margin-top: 0;*/
        /*background-color: transparent;*/
        /*border: 0;*/
        /*box-shadow: none;*/
    /*}*/

    /*.navbar-nav .open .dropdown-menu > li > a,*/
    /*.navbar-nav .open .dropdown-menu .dropdown-header {*/
        /*padding: 5px 15px 5px 25px;*/
    /*}*/

    /*.navbar-nav .open .dropdown-menu > li > a {*/
        /*line-height: 20px;*/
    /*}*/

    /*.navbar-nav .open .dropdown-menu > li > a:hover,*/
    /*.navbar-nav .open .dropdown-menu > li > a:focus {*/
        /*background-image: none;*/
    /*}*/
/*}*/

@media (min-width: 641px) {
    .navbar-nav {
        float: left;
        margin: 0;
    }

    .navbar-nav > li {
        float: left;
    }

    .navbar-nav > li > a {
        padding-top: 15px;
        padding-bottom: 15px;
    }

    .navbar-nav.navbar-right:last-child {
        margin-right: -10px;
    }
}

@media (min-width: 641px) {
    .navbar-left {
        float: left !important;
    }

    .navbar-right {
        float: right !important;
    }
}


@media screen and (min-width: 641px) {
    .carousel-control .glyphicon-chevron-left,
    .carousel-control .glyphicon-chevron-right,
    .carousel-control .icon-prev,
    .carousel-control .icon-next {
        width: 30px;
        height: 30px;
        margin-top: -15px;
        font-size: 30px;
    }

    .carousel-control .glyphicon-chevron-left,
    .carousel-control .icon-prev {
        margin-left: -15px;
    }

    .carousel-control .glyphicon-chevron-right,
    .carousel-control .icon-next {
        margin-right: -15px;
    }

    .carousel-caption {
        left: 20%;
        right: 20%;
        padding-bottom: 30px;
    }

    .carousel-indicators {
        bottom: 20px;
    }
}
/*
.center-block {
    display: block;
    margin-left: auto;
    margin-right: auto;
}

.pull-right {
    float: right !important;
}

.pull-left {
    float: left !important;
}

.hide {
    display: none !important;
}

.show {
    display: block !important;
}

.invisible {
    visibility: hidden;
}

.text-hide {
    font: 0/0 a;
    color: transparent;
    text-shadow: none;
    background-color: transparent;
    border: 0;
}

.hidden {
    display: none !important;
    visibility: hidden !important;
}

.affix {
    position: fixed;
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
}
*/
@-ms-viewport {
    width: device-width;
}
/*
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
    display: none !important;
}

.visible-xs-block,
.visible-xs-inline,
*/
.visible-xs-inline-block,

.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
    display: none !important;
}

@media (max-width: 640px) {
    .visible-xs-inline-block {
        display: inline-block !important;
    }
}

body {
    overflow-x: hidden;
}

main {
    -webkit-transition: -webkit-transform 0.3s ease-out;
    -moz-transition: -moz-transform 0.3s ease-out;
    -o-transition: -o-transform 0.3s ease-out;
    transition: transform 0.3s ease-out;
}

@media all and (min-width: 640px) and (max-width: 1023px) {
    main.offcanvas {
        -webkit-transform: translate(380px, 0);
        -ms-transform: translate(380px, 0);
        -o-transform: translate(380px, 0);
        transform: translate(380px, 0);
    }
}

/*@media (max-width: 640px) {*/
    /*main.offcanvas {*/
        /*-webkit-transform: translate(100%, 0);*/
        /*-ms-transform: translate(100%, 0);*/
        /*-o-transform: translate(100%, 0);*/
        /*transform: translate(100%, 0);*/
    /*}*/

    /*main.offcanvas > * {*/
        /*margin-left: -70px;*/
    /*}*/

    /*main.offcanvas .main-navigation {*/
        /*background: none;*/
    /*}*/

    /*main.offcanvas .main-navigation ul.nav.nav-pills {*/
        /*margin-right: 70px;*/
    /*}*/

    /*main .main-navigation {*/
        /*padding-right: 70px !important;*/
        /*width: 100% !important;*/
        /*left: -100% !important;*/
        /*z-index: -1;*/
    /*}*/

    /*main .main-navigation:before {*/
        /*content: "";*/
        /*display: block;*/
        /*position: absolute;*/
        /*top: 0;*/
        /*left: 0;*/
        /*bottom: 0;*/
        /*right: 70px;*/
        /*background: #19212b;*/
    /*}*/
/*}*/

.site-search {
    background: #fff;
    position: relative;
}

.site-search input.form-control {
    border: 0;
    box-shadow: none;
}

.site-search button {
    color: #ff4444;
    background-color: #fff;
}

.site-search button:hover,
.site-search button:focus {
    background-color: #fff;
}

@media (max-width: 640px) {
    .site-search {
        display: none;
        background: #DEE3E8;
        margin-top: 10px;
        padding: 10px;
    }

    .site-search.active {
        display: block;
    }
}

.site-search ul.ui-autocomplete {
    display: none;
    position: absolute;
    background: #fff;
    left: 0;
    right: 0;
    -webkit-box-shadow: 0 10px 0 10px rgba(0, 0, 0, 0.5);
    box-shadow: 0 10px 0 10px rgba(0, 0, 0, 0.5);
    z-index: 100;
    width: auto !important;
    padding-left: 0;
    list-style: none;
    margin: 0;
}

.site-search ul.ui-autocomplete.active {
    display: block;
}

.site-search ul.ui-autocomplete li {
    border-top: 1px solid #eee;
    display: block;
    width: 100%;
}

.site-search ul.ui-autocomplete li.ui-state-focus a {
    background: #DEE3E8;
}

.site-search ul.ui-autocomplete li a {
    display: table;
    width: 100%;
    color: inherit;
    text-decoration: none;
}

.site-search ul.ui-autocomplete li .thumb {
    display: table-cell;
    vertical-align: middle;
    padding: 0 10px 0 0;
}

.site-search ul.ui-autocomplete li .name {
    display: table-cell;
    padding: 10px;
    vertical-align: middle;
    width: 100%;
}

.site-search ul.ui-autocomplete li .thumb + .name {
    padding: 0 10px;
}

.site-search ul.ui-autocomplete li .price {
    display: table-cell;
    vertical-align: middle;
    padding: 0 10px;
}

/*@media (min-width: 641px) {*/
    /*.container {*/
        /*max-width: 1260px;*/
    /*}*/
/*}*/

.icon-arrow-left {
    position: relative;
}

.icon-arrow-left:before {
    left: 0;
    width: 14px;
    height: 15px;
    top: 0;
    background-repeat: no-repeat;
    position: absolute;
    content: "";
    background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIxNHB4IiBoZWlnaHQ9IjE1cHgiIHZpZXdCb3g9IjAgMCAxNCAxNSIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT5QYXRoPC90aXRsZT4gICAgPGRlc2M+Q3JlYXRlZCB3aXRoIFNrZXRjaC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9IkRhc2hhJ3MtRmluYWwtVmlzdWFsLURlc2lnbnMiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiPiAgICAgICAgPGcgaWQ9Ik1lbnUtMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoLTIwLjAwMDAwMCwgLTc5LjAwMDAwMCkiIGZpbGw9IiMwMDAwMDAiPiAgICAgICAgICAgIDxwYXRoIGQ9Ik0yNS45Mzc0NjMsNzkuMTcyMzA2IEMyNS42MTEyMDQxLDc4LjkwNTU4NTQgMjUuMTMwNDk5Miw3OC45NTM4NTA2IDI0Ljg2Mzc3ODUsNzkuMjgwMTA5NSBDMjQuNTk3MDU3OCw3OS42MDYzNjg0IDI0LjY0NTMyMzEsODAuMDg3MDczNCAyNC45NzE1ODIsODAuMzUzNzk0IEwzMS4wMTMyODIsODUuMjk1ODc4IEwyMCw4NS4yOTU4NzggTDIwLDg2Ljk4ODIxOSBMMzEuMDEzNzU4LDg2Ljk4ODIxOSBMMjQuOTcxNTgyLDkxLjkzMDcwOSBDMjQuNzIxNzAwMyw5Mi4xMzQ4Njg1IDI0LjYyNzIyNjUsOTIuNDc0MTIzNCAyNC43MzU2MTg0LDkyLjc3ODA1MjkgQzI0Ljg0NDAxMDIsOTMuMDgxOTgyNSAyNS4xMzE4Mzk3LDkzLjI4NDg5NDcgMjUuNDU0NTE5LDkzLjI4NDg1OSBDMjUuNjMwNzE1Miw5My4yODU0MzEgMjUuODAxNTYxNyw5My4yMjQzNTUgMjUuOTM3NDYzLDkzLjExMjIxMSBDMjUuOTM3NDYzLDkzLjExMjIxMSAzNC4wMDAyNzMsODYuMTk0MTY3IDM0LDg2LjE0MjI1NSBDMzQuMDAwMjczLDg2LjA5MDM0MyAyNS45Mzc0NjMsNzkuMTcyMzA2IDI1LjkzNzQ2Myw3OS4xNzIzMDYgWiIgaWQ9IlBhdGgiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDI3LjAwMDAwMCwgODYuMTQyNDMyKSByb3RhdGUoMTgwLjAwMDAwMCkgdHJhbnNsYXRlKC0yNy4wMDAwMDAsIC04Ni4xNDI0MzIpICI+PC9wYXRoPiAgICAgICAgPC9nPiAgICA8L2c+PC9zdmc+);
}

.icon-search-black {
    position: relative;
}

.icon-search-black:before {
    width: 22px;
    height: 22px;
    display: block;
    position: absolute;
    background-repeat: no-repeat;
    top: 0;
    left: 0;
    content: "";
    background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjIycHgiIHZpZXdCb3g9IjAgMCAyMiAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT45RjI3MjYzQy0yRjhCLTRCQjQtODJDNS02MDY4OTNGRENCNUI8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9IkZpbmFsLVZpc3VhbC1EZXNpZ25zIiBzdHJva2U9Im5vbmUiIHN0cm9rZS13aWR0aD0iMSIgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj4gICAgICAgIDxnIGlkPSJBLU1vYmlsZS1TUlAtZnVsbC1zY3JlZW4iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0yMjQuMDAwMDAwLCAtMTkuMDAwMDAwKSIgZmlsbD0iIzAwMDAwMCIgZmlsbC1ydWxlPSJub256ZXJvIj4gICAgICAgICAgICA8ZyBpZD0iR3JvdXAtMTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIyMy4wMDAwMDAsIDE4LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0ic2VhcmNoLWNvcHkiPiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIyLjQ5NDMyNjksMjEuNzA0MjM1MyBMMTUuMTQ5MTY2OSwxNC4zNTkwODUzIEMxNy45OTYzNTgzLDExLjA4Njk4NzUgMTcuNzQ1Njk4MSw2LjE0OTAwNDczIDE0LjU4MTgwMTQsMy4xODIwMzk4MiBDMTEuNDE3OTA0NywwLjIxNTA3NDkwOCA2LjQ3NDAxNDc4LDAuMjgxODM0MDg4IDMuMzkxMzg1MTUsMy4zMzMxNDgxNiBDMC4zMDg3NTU1MjEsNi4zODQ0NjIyNCAwLjE5MTUyMTE2MiwxMS4zMjc0MTI4IDMuMTI2MDI3MDQsMTQuNTIxNDM4MiBDNi4wNjA1MzI5MiwxNy43MTU0NjM2IDEwLjk5NTY5OSwxOC4wMTY1MjkyIDE0LjI5NjY5NjksMTUuMjAyODk1MyBMMjEuNjQ2Njk2OSwyMi41NTI4OTUzIEMyMS44ODExNTIzLDIyLjc4NjMwOSAyMi4yNjAzMzksMjIuNzg1Nzc4NCAyMi40OTQxNDA0LDIyLjU1MTcwOTYgQzIyLjcyNzk0MTcsMjIuMzE3NjQwNyAyMi43MjgwMzg2LDIxLjkzODQ1MzYgMjIuNDk0MzU2OSwyMS43MDQyNjUzIEwyMi40OTQzMjY5LDIxLjcwNDIzNTMgWiBNMi4xNjQyNDY5MSw5LjAyOTkxNTI5IEMyLjE2NDA1Mjc2LDYuMjM4OTI0MzggMy44NDUxNTU3MiwzLjcyMjY0NDQ4IDYuNDIzNjM5MzYsMi42NTQ0NDM5OCBDOS4wMDIxMjMwMSwxLjU4NjI0MzQ3IDExLjk3MDE4MjUsMi4xNzY0OTMwNiAxMy45NDM3Nzk3LDQuMTQ5OTUzMDIgQzE1LjkxNzM3Nyw2LjEyMzQxMjk3IDE2LjUwNzgzMyw5LjA5MTQzMTM5IDE1LjQzOTgxMTksMTEuNjY5OTg5MyBDMTQuMzcxNzkwOCwxNC4yNDg1NDczIDExLjg1NTYyNzgsMTUuOTI5ODI1MyA5LjA2NDYzNjkxLDE1LjkyOTgyNTMgQzUuMjU1NTgyNDcsMTUuOTI1NjMxOCAyLjE2ODcwNTQxLDEyLjgzODk2OTQgMi4xNjQyNDY5MSw5LjAyOTkxNTI5IFoiIGlkPSJTaGFwZSI+PC9wYXRoPiAgICAgICAgICAgICAgICA8L2c+ICAgICAgICAgICAgPC9nPiAgICAgICAgPC9nPiAgICA8L2c+PC9zdmc+);
}

/*@media (max-width: 640px) {*/
    /*.my-account .icon-email {*/
        /*background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACEAAAAZCAYAAAC/zUevAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAyJpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMy1jMDExIDY2LjE0NTY2MSwgMjAxMi8wMi8wNi0xNDo1NjoyNyAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvIiB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RSZWY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENTNiAoV2luZG93cykiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6RTQzM0MyMDQ2OUU4MTFFNjhGNEJGMDM0M0U0RjdERTciIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6RTQzM0MyMDU2OUU4MTFFNjhGNEJGMDM0M0U0RjdERTciPiA8eG1wTU06RGVyaXZlZEZyb20gc3RSZWY6aW5zdGFuY2VJRD0ieG1wLmlpZDpFNDMzQzIwMjY5RTgxMUU2OEY0QkYwMzQzRTRGN0RFNyIgc3RSZWY6ZG9jdW1lbnRJRD0ieG1wLmRpZDpFNDMzQzIwMzY5RTgxMUU2OEY0QkYwMzQzRTRGN0RFNyIvPiA8L3JkZjpEZXNjcmlwdGlvbj4gPC9yZGY6UkRGPiA8L3g6eG1wbWV0YT4gPD94cGFja2V0IGVuZD0iciI/PkAkWrgAAAFZSURBVHja7Je7agJBFIZPVCIIIikkTbAIgjYBu/Q2FkIqu1S+Ut4hlVbpRBBbwUIIFoJgk0BEEAwhBDdx/AfOLMPgZXZnMVt44Ft253Lm29nbLAkhcqANPHHa8Hjc3AU2LSJq0P9FW0p42EmBHzADJZDgBl9ctnEYJANuQZKPP8AclEEa/JI2PX0gj6vgWyvvgQzXBeUOLLVcA5DlupEq3CURlUgZLLQcr3z/ka2EpA7WIUWK4E3rOwZ5o42VhOTBEOmCyyMCN2Cm9ZlyGYWV2CXyckDkmgdVIWejsKdtIAlbkTxfdxXvfFkoKoljIvKGG2p1C34yKGqJfSJX/OipWIGKRa7QEpIG+DPOWsUnuLfM4yQheTREBL9XqgFyOEsoERUbUAvY35dIOXwTnvk70wRPoBM6k8NMuOLPRIJiEGeJs0QsJcw15uSEY/trzFistikO/x1bAQYAxddTCklsAPUAAAAASUVORK5CYII=);*/
    /*}*/

    /*.my-account .icon-print2 {*/
        /*background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABoAAAAaCAYAAACpSkzOAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAyJpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMy1jMDExIDY2LjE0NTY2MSwgMjAxMi8wMi8wNi0xNDo1NjoyNyAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvIiB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RSZWY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENTNiAoV2luZG93cykiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6QUI1ODZGQTA2OUVDMTFFNjhBMTFDNEI3NkZDNTcyM0MiIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6QUI1ODZGQTE2OUVDMTFFNjhBMTFDNEI3NkZDNTcyM0MiPiA8eG1wTU06RGVyaXZlZEZyb20gc3RSZWY6aW5zdGFuY2VJRD0ieG1wLmlpZDpBQjU4NkY5RTY5RUMxMUU2OEExMUM0Qjc2RkM1NzIzQyIgc3RSZWY6ZG9jdW1lbnRJRD0ieG1wLmRpZDpBQjU4NkY5RjY5RUMxMUU2OEExMUM0Qjc2RkM1NzIzQyIvPiA8L3JkZjpEZXNjcmlwdGlvbj4gPC9yZGY6UkRGPiA8L3g6eG1wbWV0YT4gPD94cGFja2V0IGVuZD0iciI/PtEJM4gAAADeSURBVHjaYvj//z8DGp75n3IwE91cRhCBBjAEyASMyBwWPApnAfEWEg33AeI0bBIsBDRuJsMirICJgU6AbhZhSww089FMaEqjJZ4J8tH/oRxHoDx0ETkv0cqiC0CsD6XhieE/jXwEssQAVtLgyrAXKbToP0ZxhqVAvECFQvUAugALsYUiGb4hqaz7T0bcDHxZN4sO9sxiwFLDwhIDAxmJgAEpMaCYy8TIyEiXoAMnBmTLqJV/0T0w/Co+FnLzBTV89AAps5KDQeAl4fLj/39dIL5JQTl3BYg10M0FCDAAGiqxqD1+LNMAAAAASUVORK5CYII=);*/
    /*}*/
/*}*/

@media (min-width: 641px) {
    .icon-download-dark-teal {
        padding: 0 31px;
    }

    .icon-download-dark-teal:before {
        background-size: 18px auto;
    }
}



/*.main-header-container {*/
    /*font-family: 'Open Sans', sans-serif;*/
    /*position: relative;*/
    /*font-size: 10px;*/
    /*margin-bottom: 0;*/
    /*height: 156px;*/
    /*z-index: 1000;*/
/*}*/

/*.main-header-container a:focus,*/
/*.main-header-container a:hover {*/
    /*color: inherit;*/
/*}*/

.main-header-container .main-sticky-header {
    background: darkgrey;
    padding: 0;
    position: fixed;
    width: 100%;
}

.main-header-container .main-sticky-header.affix {
    box-shadow: 0 16px 16px -7px rgba(0, 0, 0, 0.09);
}

.main-header-container .main-navigation-menu {
    overflow-x: visible;
}

.main-header-container .navigation-links-items {
    display: flex;
    align-items: center;
    font-family: 'Open Sans', sans-serif;
    font-size: 1.2em;
    position: relative;
    margin-bottom: 0;
}

.main-header-container .navigation-links-items .navigation-link-item {
    display: block;
    margin-left: 28px;
    list-style: none;
    color: #dddedf;
    top: 2px;
    position: relative;
}

.main-header-container .navigation-links-items .navigation-link-item:first-child {
    margin-left: 0;
}

.main-header-container .navigation-links-items .navigation-link-item > a {
    letter-spacing: -0.29px;
    white-space: nowrap;
    color: rgba(0, 0, 0, 0.87);
}

.main-header-container .navigation-links-items .navigation-link-item > a:hover,
.main-header-container .navigation-links-items .navigation-link-item > a:focus {
    cursor: pointer;
    color: #009ca9;
    text-decoration: underline;
}

.main-header-container .navigation-links-items .navigation-link-item > a:hover span,
.main-header-container .navigation-links-items .navigation-link-item > a:focus span {
    color: inherit;
}

/*.main-header-container .main-navigation-search {*/
    /*height: 48px;*/
    /*padding: 24px 0;*/
    /*position: relative;*/
    /*z-index: 1;*/
    /*box-sizing: content-box;*/
/*}*/

/*.main-header-container .main-navigation-search > .container {*/
    /*max-width: 840px;*/
/*}*/

/*.main-header-container .main-navigation-search .input-group {*/
    /*width: 100%;*/
/*}*/

/*.main-header-container .main-navigation-search .input-group .input-group-btn button {*/
    /*width: 48px;*/
    /*height: 48px;*/
    /*background-color: #414245;*/
    /*outline: none;*/
    /*cursor: pointer;*/
    /*font-size: 0;*/
    /*transition: background-color, 0.3s, linear;*/
    /*border: none;*/
    /*background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjIycHgiIHZpZXdCb3g9IjAgMCAyMiAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT42MDQ5N0NENC1BMEZFLTQwQzctQUU0NC1GMEQzMDZBQkJDMjA8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxnIGlkPSJGaW5hbC1WaXN1YWwtRGVzaWducyIgc3Ryb2tlPSJub25lIiBzdHJva2Utd2lkdGg9IjEiIGZpbGw9Im5vbmUiIGZpbGwtcnVsZT0iZXZlbm9kZCI+ICAgICAgICA8ZyBpZD0iSG9tZS1QYWdlX0Jhbm5lci1BbGlnbmVkLUxlZnQtIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTA5NS4wMDAwMDAsIC05Ny4wMDAwMDApIiBmaWxsPSIjRkZGRkZGIiBmaWxsLXJ1bGU9Im5vbnplcm8iPiAgICAgICAgICAgIDxnIGlkPSJTZWFyY2giIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMxMC4wMDAwMDAsIDg0LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0iSWNvbl9TZWFyY2giIHRyYW5zZm9ybT0idHJhbnNsYXRlKDc4NS4wMDAwMDAsIDEzLjAwMDAwMCkiPiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIxLjQ5NDMyNjksMjAuNzA0MjM1MyBMMTQuMTQ5MTY2OSwxMy4zNTkwODUzIEMxNi45OTYzNTgzLDEwLjA4Njk4NzUgMTYuNzQ1Njk4MSw1LjE0OTAwNDczIDEzLjU4MTgwMTQsMi4xODIwMzk4MiBDMTAuNDE3OTA0NywtMC43ODQ5MjUwOTIgNS40NzQwMTQ3OCwtMC43MTgxNjU5MTIgMi4zOTEzODUxNSwyLjMzMzE0ODE2IEMtMC42OTEyNDQ0NzksNS4zODQ0NjIyNCAtMC44MDg0Nzg4MzgsMTAuMzI3NDEyOCAyLjEyNjAyNzA0LDEzLjUyMTQzODIgQzUuMDYwNTMyOTIsMTYuNzE1NDYzNiA5Ljk5NTY5ODk1LDE3LjAxNjUyOTIgMTMuMjk2Njk2OSwxNC4yMDI4OTUzIEwyMC42NDY2OTY5LDIxLjU1Mjg5NTMgQzIwLjg4MTE1MjMsMjEuNzg2MzA5IDIxLjI2MDMzOSwyMS43ODU3Nzg0IDIxLjQ5NDE0MDQsMjEuNTUxNzA5NiBDMjEuNzI3OTQxNywyMS4zMTc2NDA3IDIxLjcyODAzODYsMjAuOTM4NDUzNiAyMS40OTQzNTY5LDIwLjcwNDI2NTMgTDIxLjQ5NDMyNjksMjAuNzA0MjM1MyBaIE0xLjE2NDI0NjkxLDguMDI5OTE1MjkgQzEuMTY0MDUyNzYsNS4yMzg5MjQzOCAyLjg0NTE1NTcyLDIuNzIyNjQ0NDggNS40MjM2MzkzNiwxLjY1NDQ0Mzk4IEM4LjAwMjEyMzAxLDAuNTg2MjQzNDcgMTAuOTcwMTgyNSwxLjE3NjQ5MzA2IDEyLjk0Mzc3OTcsMy4xNDk5NTMwMiBDMTQuOTE3Mzc3LDUuMTIzNDEyOTcgMTUuNTA3ODMzLDguMDkxNDMxMzkgMTQuNDM5ODExOSwxMC42Njk5ODkzIEMxMy4zNzE3OTA4LDEzLjI0ODU0NzMgMTAuODU1NjI3OCwxNC45Mjk4MjUzIDguMDY0NjM2OTEsMTQuOTI5ODI1MyBDNC4yNTU1ODI0NywxNC45MjU2MzE4IDEuMTY4NzA1NDEsMTEuODM4OTY5NCAxLjE2NDI0NjkxLDguMDI5OTE1MjkgWiIgaWQ9IlNoYXBlIj48L3BhdGg+ICAgICAgICAgICAgICAgIDwvZz4gICAgICAgICAgICA8L2c+ICAgICAgICA8L2c+ICAgIDwvZz48L3N2Zz4=);*/
    /*background-repeat: no-repeat;*/
    /*background-position: center;*/
    /*background-size: 24px;*/
/*}*/

.main-header-container .main-navigation-search .input-group .input-group-btn button:hover {
    outline: none;
    background-color: #00b1c2;
    color: darkorange;
    color: #414245;
    box-shadow: none;
    border-color: #00b1c2;
}

/*.main-header-container .main-navigation-search .input-group .main-navigation-search-input {*/
    /*width: 100%;*/
    /*height: 48px;*/
    /*padding: 0 14px;*/
    /*font-size: 1.6em;*/
    /*background: none;*/
    /*box-shadow: none;*/
    /*border: 1px solid #c2c3c6;*/
    /*border-right: none;*/
/*}*/

/*.main-header-container .main-navigation-search .input-group .main-navigation-search-input::placeholder {*/
    /*color: #d8d9da;*/
/*}*/

/*.main-header-container .main-navigation-search .input-group .main-navigation-search-input::-ms-clear {*/
    /*display: none;*/
/*}*/

/*.main-header-container .main-navigation-search-autocomplete {*/
    /*position: relative;*/
    /*max-height: calc(100vh - 125px);*/
    /*width: auto !important;*/
    /*margin-top: -1px;*/
    /*padding: 20px 20px 5px;*/
    /*font-family: 'Open Sans', sans-serif;*/
    /*letter-spacing: 0.24px;*/
    /*background: white;*/
    /*border: 1px solid #979797;*/
    /*overflow-y: auto;*/
/*}*/

.main-header-container .main-navigation-search-autocomplete::-webkit-scrollbar {
    width: 7px;
}

.main-header-container .main-navigation-search-autocomplete::-webkit-scrollbar-track {
    -webkit-box-shadow: inset 0 0 4px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
}

.main-header-container .main-navigation-search-autocomplete::-webkit-scrollbar-thumb {
    border-radius: 10px;
    color: #dddedf;
    background: #dddedf;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section {
    padding-bottom: 18px;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section > * {
    padding: 0;
    margin: 0;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a {
    color: #414245;
    text-transform: capitalize;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a b,
.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a span,
.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a .search-highlight {
    color: #BCBCBF;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section h3 {
    margin: 0 0 4px;
    text-transform: uppercase;
    font-size: 16px;
    line-height: 22px;
    color: #96969B;
    font-weight: 700;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-list {
    list-style: none;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item {
    padding: 0;
    font-size: 14px;
    line-height: 34px;
    font-weight: 400;
    color: #000000;
    white-space: nowrap;
    text-overflow: ellipsis;
    overflow: hidden;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item:last-of-type,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item:last-of-type {
    padding-bottom: 0;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item a,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item a {
    color: rgba(0, 0, 0, 0.87);
    font-weight: 400;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item a:hover,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item a:hover {
    text-decoration: underline;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item a b,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item a b {
    font-weight: 400;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item.ui-state-focused a,
.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item.ui-state-focused a {
    outline: 5px auto Highlight;
    outline: 5px auto -webkit-focus-ring-color;
    outline-offset: -5px;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .all-results-link,
.main-header-container .main-navigation-search-autocomplete .searchresults-section a.all-results-link {
    display: inline-block;
    margin-top: 7px;
    margin-bottom: 10px;
    font-size: 14px;
    font-weight: 600;
    line-height: 1.2;
    color: #1AA6B1;
    cursor: pointer;
}

.main-header-container .main-navigation-search-autocomplete .searchresults-section .all-results-link .ui-state-focused,
.main-header-container .main-navigation-search-autocomplete .searchresults-section a.all-results-link .ui-state-focused {
    outline: 5px auto Highlight;
    outline: 5px auto -webkit-focus-ring-color;
    outline-offset: -5px;
}

.main-header-container .shopping-cart-icon {
    background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjI0cHgiIHZpZXdCb3g9IjAgMCAyMiAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT4yRDNCQTg5OS03RENDLTQxNzgtQUQ1OS1CQzFEODE4MDBERTM8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9IkZpbmFsLVZpc3VhbC1EZXNpZ25zIiBzdHJva2U9Im5vbmUiIHN0cm9rZS13aWR0aD0iMSIgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj4gICAgICAgIDxnIGlkPSJBLU1vYmlsZS1TUlAtZnVsbC1zY3JlZW4iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0yNzMuMDAwMDAwLCAtMTguMDAwMDAwKSIgZmlsbD0iIzAwMDAwMCIgZmlsbC1ydWxlPSJub256ZXJvIj4gICAgICAgICAgICA8ZyBpZD0iR3JvdXAtMTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIyMy4wMDAwMDAsIDE4LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0iSWNvbl9CYWciIHRyYW5zZm9ybT0idHJhbnNsYXRlKDUwLjAwMDAwMCwgMC4wMDAwMDApIj4gICAgICAgICAgICAgICAgICAgIDxnIGlkPSJjYXJ0Ij4gICAgICAgICAgICAgICAgICAgICAgICA8cGF0aCBkPSJNMTguNDA0LDIzLjI4MDExIEMxOS4yNjA5MTE1LDIzLjI4MTg2MDkgMjAuMDUzNDgwNiwyMi44MjU3MDkzIDIwLjQ4MjQ0MjYsMjIuMDgzODkyNSBDMjAuOTExNDA0NiwyMS4zNDIwNzU4IDIwLjkxMTQwNDYsMjAuNDI3NjE0MiAyMC40ODI0NDI2LDE5LjY4NTc5NzUgQzIwLjA1MzQ4MDYsMTguOTQzOTgwNyAxOS4yNjA5MTE1LDE4LjQ4NzgyOTEgMTguNDA0LDE4LjQ4OTU4IEw2LjMwMjQzLDE4LjQ5MDU4IEM1Ljg4NDQzLDE4LjQ2NzY0IDUuMTA2MTQsMTguMjMyNzcgNS4xMDYxNCwxNy41MDgxNiBMNS4xMDYxNCwxNS42MTIxNiBMNS4yOTU2LDE1LjcyNTQ0IEM1LjY4MjQ1MzA5LDE1Ljk2MjQ2MjUgNi4xMjcwNjEyMSwxNi4wODg0ODEzIDYuNTgwNzUsMTYuMDg5NyBMMTguOTMyMzYsMTYuMDg5NyBDMjAuMzI2Mjk3MiwxNi4wODgyMjg5IDIxLjQ1NjAxMzksMTQuOTU4NzI2OSAyMS40NTc3NSwxMy41NjQ3OSBMMjEuNDU3NzUsOC4yNjgzOSBDMjEuNDU1OTk3Miw3Ljc1NTcyMzQ0IDIxLjA3NjIwMzUsNy4zMjI5ODEwMiAyMC41NjgxLDcuMjU0NzEgTDUuMTA2MTgsNS4yMjQ0NCBMNS4xMDYxOCwzLjAwMDMyIEM1LjEwNzc3MDY4LDIuNTczMDgxMjQgNC44NDcyODUyMiwyLjE4ODU1NTA4IDQuNDQ5OTMsMi4wMzE1NyBMMS4yNjI0MywwLjc1ODU3IEMxLjEzMzE4NTA2LDAuNzA2MTI3NzQyIDAuOTg4MzM4ODQ0LDAuNzA3NTI5MDEzIDAuODYwMTMyNjc1LDAuNzYyNDYxOTA0IEMwLjczMTkyNjUwNSwwLjgxNzM5NDc5NSAwLjYzMTAwMDU3OCwwLjkyMTMwMDI2OSAwLjU3OTgyLDEuMDUxMDUgQzAuNDcyMjgzMywxLjMyMDA0NjI1IDAuNjAyOTU3NTIxLDEuNjI1MzA5MjggMC44NzE4MiwxLjczMzE4IEw0LjA1NTQsMy4wMDUyIEw0LjA1NTQsMTcuNTA4MTMgQzQuMTE3NTkzODEsMTguNjc1MjY5MiA1LjEwMjA5ODU1LDE5LjU3ODE2MzQgNi4yNzAyNSwxOS41MzkzOCBMNi45MzEzOCwxOS41MzkzOCBMNi44MjY4OSwxOS43MjUzOCBDNi42MjM1MjcwMiwyMC4wNzgxODEzIDYuNTE1NDkyMjgsMjAuNDc3ODM4OSA2LjUxMzQxLDIwLjg4NTA1IEM2LjUxNzIyNDk1LDIyLjIwNTM0NTggNy41ODg2MDg2NSwyMy4yNzM2MzgzIDguOTA4OTEsMjMuMjczNjM4MyBDMTAuMjI5MjExMywyMy4yNzM2MzgzIDExLjMwMDU5NTEsMjIuMjA1MzQ1OCAxMS4zMDQ0MSwyMC44ODUwNSBDMTEuMzAxOTUwNiwyMC40Nzc4OSAxMS4xOTM5NDE1LDIwLjA3ODMyNzEgMTAuOTkwOTMsMTkuNzI1MzggTDEwLjg4NzQxLDE5LjUzOTM4IEwxNi40MjY1LDE5LjUzOTM4IEwxNi4zMjIsMTkuNzI1MzggQzE2LjExODY0NDQsMjAuMDc4MTgzOCAxNi4wMTA2MTM0LDIwLjQ3Nzg0MDMgMTYuMDA4NTMsMjAuODg1MDUgQzE2LjAwOTkzMDQsMjIuMjA3Mzg0NyAxNy4wODE2NjUxLDIzLjI3ODkzNiAxOC40MDQsMjMuMjgwMTEgWiBNMTguNDA0LDE5LjUzOTM4IEMxOC45NDgyMzE0LDE5LjUzOTA4NDcgMTkuNDM5MDQzMSwxOS44NjY2ODEyIDE5LjY0NzUzOTQsMjAuMzY5MzkxIEMxOS44NTYwMzU3LDIwLjg3MjEwMDggMTkuNzQxMTQ5OSwyMS40NTA5MDcyIDE5LjM1NjQ2MDMsMjEuODM1ODc3MSBDMTguOTcxNzcwOCwyMi4yMjA4NDcgMTguMzkzMDQ4MywyMi4zMzYxNTQ0IDE3Ljg5MDE4NjcsMjIuMTI4MDI0NCBDMTcuMzg3MzI1MiwyMS45MTk4OTQzIDE3LjA1OTM3MTIsMjEuNDI5MzIxNCAxNy4wNTkyNywyMC44ODUwOSBDMTcuMDU5OTgwMSwyMC4xNDI1NTE3IDE3LjY2MTQ2MjQsMTkuNTQwNjMxIDE4LjQwNCwxOS41MzkzOCBaIE01LjEwNjE4LDYuMjgyNTUgTDIwLjQwNyw4LjI5MjMxIEwyMC40MDcsMTMuNTY0NzcgQzIwLjQwNjM4MjcsMTQuMzc4OTk4MSAxOS43NDY2MTc5LDE1LjAzODk4MjIgMTguOTMyMzksMTUuMDM5ODcgTDYuNTgwNzksMTUuMDM5ODcgQzUuNzY2NTYyMTEsMTUuMDM4OTgyMiA1LjEwNjc5NzI3LDE0LjM3ODk5ODEgNS4xMDYxOCwxMy41NjQ3NyBMNS4xMDYxOCw2LjI4MjU1IFogTTguOTA4OTIsMjIuMjMwMyBDOC4zNjQ2NDMxNSwyMi4yMzA1OTUzIDcuODczNzk5NzksMjEuOTAyOTQ0NyA3LjY2NTMzMjc2LDIxLjQwMDE3MzUgQzcuNDU2ODY1NzQsMjAuODk3NDAyMyA3LjU3MTg0MzE1LDIwLjMxODU1NjcgNy45NTY2MzYzOCwxOS45MzM2MjYxIEM4LjM0MTQyOTYxLDE5LjU0ODY5NTUgOC45MjAyMzQxOSwxOS40MzM1MTE1IDkuNDIzMDc5NzYsMTkuNjQxNzk5MSBDOS45MjU5MjUzMywxOS44NTAwODY3IDEwLjI1Mzc1MTEsMjAuMzQwODEzMSAxMC4yNTM2NSwyMC44ODUwOSBDMTAuMjUyODIzOSwyMS42Mjc0OTkyIDkuNjUxMzI4ODMsMjIuMjI5MjA4OSA4LjkwODkyLDIyLjIzMDMgWiIgaWQ9IlNoYXBlIj48L3BhdGg+ICAgICAgICAgICAgICAgICAgICA8L2c+ICAgICAgICAgICAgICAgIDwvZz4gICAgICAgICAgICA8L2c+ICAgICAgICA8L2c+ICAgIDwvZz48L3N2Zz4=);
    width: 22px;
    display: block;
    height: 24px;
    background-size: contain;
    background-repeat: no-repeat;
}

.page-productSearchPage .main-sticky-header.affix {
    box-shadow: none;
}

.ui-selectmenu-menu {
    z-index: 9999;
}

/*@media (max-width: 640px) {*/
    /*.main-header-container {*/
        /*margin: 0;*/
        /*height: 60px;*/
    /*}*/

    /*.main-header-container .main-sticky-header {*/
        /*height: 60px;*/
        /*box-shadow: 0px 8px 8px -7px rgba(0, 0, 0, 0.19);*/
    /*}*/

    /*.main-header-container .main-sticky-header.no-shadow,*/
    /*.main-header-container .main-sticky-header.no-shadow.affix {*/
        /*box-shadow: none;*/
    /*}*/

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

    /*.main-header-container .main-navigation-search {*/
        /*position: fixed;*/
        /*top: -100px;*/
        /*width: 100%;*/
        /*height: 52px;*/
        /*padding: 0;*/
        /*box-sizing: border-box;*/
        /*transition: all 0.5s ease-out;*/
        /*-webkit-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
        /*-moz-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
        /*box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
    /*}*/

    /*.main-header-container .main-navigation-search.open {*/
        /*top: 60px;*/
    /*}*/

    /*.main-header-container .main-navigation-search > .container {*/
        /*padding: 0;*/
    /*}*/

    /*.main-header-container .main-navigation-search > .container:after,*/
    /*.main-header-container .main-navigation-search > .container:before {*/
        /*display: none;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group {*/
        /*background-color: #efeff0;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .input-group-btn button {*/
        /*height: 52px;*/
        /*width: 40px;*/
        /*padding-right: 20px;*/
        /*background-color: unset;*/
        /*font-style: normal;*/
        /*font-weight: normal;*/
        /*background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyMnB4IiBoZWlnaHQ9IjIycHgiIHZpZXdCb3g9IjAgMCAyMiAyMiIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT45RjI3MjYzQy0yRjhCLTRCQjQtODJDNS02MDY4OTNGRENCNUI8L3RpdGxlPiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggc2tldGNodG9vbC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9IkZpbmFsLVZpc3VhbC1EZXNpZ25zIiBzdHJva2U9Im5vbmUiIHN0cm9rZS13aWR0aD0iMSIgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj4gICAgICAgIDxnIGlkPSJBLU1vYmlsZS1TUlAtZnVsbC1zY3JlZW4iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0yMjQuMDAwMDAwLCAtMTkuMDAwMDAwKSIgZmlsbD0iIzAwMDAwMCIgZmlsbC1ydWxlPSJub256ZXJvIj4gICAgICAgICAgICA8ZyBpZD0iR3JvdXAtMTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIyMy4wMDAwMDAsIDE4LjAwMDAwMCkiPiAgICAgICAgICAgICAgICA8ZyBpZD0ic2VhcmNoLWNvcHkiPiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIyLjQ5NDMyNjksMjEuNzA0MjM1MyBMMTUuMTQ5MTY2OSwxNC4zNTkwODUzIEMxNy45OTYzNTgzLDExLjA4Njk4NzUgMTcuNzQ1Njk4MSw2LjE0OTAwNDczIDE0LjU4MTgwMTQsMy4xODIwMzk4MiBDMTEuNDE3OTA0NywwLjIxNTA3NDkwOCA2LjQ3NDAxNDc4LDAuMjgxODM0MDg4IDMuMzkxMzg1MTUsMy4zMzMxNDgxNiBDMC4zMDg3NTU1MjEsNi4zODQ0NjIyNCAwLjE5MTUyMTE2MiwxMS4zMjc0MTI4IDMuMTI2MDI3MDQsMTQuNTIxNDM4MiBDNi4wNjA1MzI5MiwxNy43MTU0NjM2IDEwLjk5NTY5OSwxOC4wMTY1MjkyIDE0LjI5NjY5NjksMTUuMjAyODk1MyBMMjEuNjQ2Njk2OSwyMi41NTI4OTUzIEMyMS44ODExNTIzLDIyLjc4NjMwOSAyMi4yNjAzMzksMjIuNzg1Nzc4NCAyMi40OTQxNDA0LDIyLjU1MTcwOTYgQzIyLjcyNzk0MTcsMjIuMzE3NjQwNyAyMi43MjgwMzg2LDIxLjkzODQ1MzYgMjIuNDk0MzU2OSwyMS43MDQyNjUzIEwyMi40OTQzMjY5LDIxLjcwNDIzNTMgWiBNMi4xNjQyNDY5MSw5LjAyOTkxNTI5IEMyLjE2NDA1Mjc2LDYuMjM4OTI0MzggMy44NDUxNTU3MiwzLjcyMjY0NDQ4IDYuNDIzNjM5MzYsMi42NTQ0NDM5OCBDOS4wMDIxMjMwMSwxLjU4NjI0MzQ3IDExLjk3MDE4MjUsMi4xNzY0OTMwNiAxMy45NDM3Nzk3LDQuMTQ5OTUzMDIgQzE1LjkxNzM3Nyw2LjEyMzQxMjk3IDE2LjUwNzgzMyw5LjA5MTQzMTM5IDE1LjQzOTgxMTksMTEuNjY5OTg5MyBDMTQuMzcxNzkwOCwxNC4yNDg1NDczIDExLjg1NTYyNzgsMTUuOTI5ODI1MyA5LjA2NDYzNjkxLDE1LjkyOTgyNTMgQzUuMjU1NTgyNDcsMTUuOTI1NjMxOCAyLjE2ODcwNTQxLDEyLjgzODk2OTQgMi4xNjQyNDY5MSw5LjAyOTkxNTI5IFoiIGlkPSJTaGFwZSI+PC9wYXRoPiAgICAgICAgICAgICAgICA8L2c+ICAgICAgICAgICAgPC9nPiAgICAgICAgPC9nPiAgICA8L2c+PC9zdmc+);*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .input-group-btn button:before {*/
        /*top: 0;*/
        /*bottom: 0;*/
        /*margin: auto;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .input-group-btn button:focus {*/
        /*background-color: unset;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .main-navigation-search-input {*/
        /*height: 52px;*/
        /*padding: 0 15px;*/
        /*font-size: 1.3em;*/
        /*font-weight: 600;*/
        /*color: #000000;*/
        /*border: none;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .main-navigation-search-input::placeholder {*/
        /*color: #979797;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .main-navigation-search-input:focus + .input-group-btn button {*/
        /*background-color: unset;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete {*/
        /*max-height: calc(100vh - 212px);*/
        /*max-height: calc(var(--vh, 1vh) * 100 - 212px);*/
        /*margin-top: 0;*/
        /*padding: 15px 15px 5px;*/
        /*!*border: 1px solid #dddedf;*!*/
        /*border-left: none;*/
        /*border-right: none;*/
        /*-webkit-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
        /*-moz-box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
        /*box-shadow: 0 10px 10px 0 rgba(67, 99, 125, 0.11);*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section {*/
        /*padding-bottom: 20px;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a {*/
        /*font-weight: 700;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section.suggestions .searchresults-item a b {*/
        /*color: rgba(0, 0, 0, 0.87);*/
        /*font-weight: 400;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section .searchresults-item,*/
    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section .ui-menu-item {*/
        /*line-height: 2.2;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section h3 {*/
        /*margin-bottom: 5px;*/
    /*}*/

    /*.main-header-container .main-navigation-search-autocomplete .searchresults-section .all-results-link {*/
        /*font-weight: 600;*/
        /*color: #1AA6B1;*/
        /*text-decoration: none;*/
    /*}*/

    /*.main-header-container .main-navigation-mobile-header {*/
        /*z-index: 2;*/
        /*height: 60px;*/
        /*position: relative;*/
        /*padding: 0 0 0 20px;*/
        /*display: flex;*/
        /*align-items: center;*/
        /*justify-content: flex-end;*/
        /*background: white;*/
        /*!*border-bottom: 1px solid #dddedf;*!*/
    /*}*/

    /*.main-header-container .main-navigation-mobile-header .my-cart-link {*/
        /*margin: 0 20px 0 20px;*/
    /*}*/

    /*.main-header-container .main-navigation-mobile-header .logo {*/
        /*margin-right: auto;*/
    /*}*/

    /*.main-header-container .main-navigation-mobile-header .logo .simple-responsive-banner-component {*/
        /*margin: 0;*/
    /*}*/

    /*.main-header-container .main-navigation-mobile-header .logo a,*/
    /*.main-header-container .main-navigation-mobile-header .logo img {*/
        /*width: 90px;*/
        /*height: 20px;*/
    /*}*/

    /*.main-header-container .navigation-links-items {*/
        /*margin: 0;*/
        /*padding: 0;*/
        /*position: static;*/
        /*display: block;*/
    /*}*/

    /*.main-header-container .navigation-links-items .navigation-link-item {*/
        /*margin-left: 15px;*/
        /*padding: 10px 0;*/
    /*}*/

    /*.main-header-container .navigation-links-items .navigation-link-item:first-child {*/
        /*margin-left: 15px;*/
    /*}*/

    /*.main-header-container .navigation-links-items .navigation-link-item.my-account-link {*/
        /*position: absolute;*/
        /*right: 20px;*/
        /*bottom: 10px;*/
        /*top: unset;*/
        /*line-height: 44px;*/
        /*padding-bottom: 0;*/
        /*margin: 0;*/
        /*font-size: 16px;*/
    /*}*/

    /*.main-header-container .navigation-links-items .navigation-link-item.my-account-link:before {*/
        /*content: "";*/
        /*width: 17px;*/
        /*height: 19px;*/
        /*margin-right: 5px;*/
        /*background-size: contain;*/
        /*background-repeat: no-repeat;*/
        /*vertical-align: middle;*/
        /*display: inline-block;*/
        /*background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyNHB4IiBoZWlnaHQ9IjI0cHgiIHZpZXdCb3g9IjAgMCAyNCAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4gICAgICAgIDx0aXRsZT5NeSBhY2NvdW50PC90aXRsZT4gICAgPGRlc2M+Q3JlYXRlZCB3aXRoIFNrZXRjaC48L2Rlc2M+ICAgIDxkZWZzPjwvZGVmcz4gICAgPGcgaWQ9Ik15LWFjY291bnQiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiPiAgICAgICAgPGcgaWQ9Ikdyb3VwLTIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDYuMDAwMDAwLCAzLjAwMDAwMCkiIGZpbGwtcnVsZT0ibm9uemVybyIgc3Ryb2tlPSIjMDAwMDAwIj4gICAgICAgICAgICA8Y2lyY2xlIGlkPSJPdmFsIiBjeD0iNiIgY3k9IjYiIHI9IjYiPjwvY2lyY2xlPiAgICAgICAgPC9nPiAgICAgICAgPHBhdGggZD0iTTguNjQyNDU2MDUsMTQuMjg0MTc5NyBDNS4xNTc3NTU1MywxOC4xMTAwNjM1IDMuNDE1NDA1MjcsMjAuODIxMzI2NSAzLjQxNTQwNTI3LDIyLjQxNzk2ODcgQzcuMDk4MjY2NiwyMi40MTc5Njg3IDE2LjcwOTU5NDcsMjIuNDE3OTY4NyAyMC41NzU1NjE1LDIyLjQxNzk2ODcgQzIwLjU3NTU2MTUsMjAuODYxMzYwMiAxOC43ODM4OTQ5LDE4LjE1MDA5NzIgMTUuMjAwNTYxNSwxNC4yODQxNzk3IiBpZD0iTGluZS00IiBzdHJva2U9IiMwMDAwMDAiIHN0cm9rZS1saW5lY2FwPSJzcXVhcmUiPjwvcGF0aD4gICAgPC9nPjwvc3ZnPg==);*/
    /*}*/

    /*.main-header-container .navbar-collapse {*/
        /*margin: 0;*/
        /*padding: 0;*/
        /*border-top: none;*/
        /*width: 100%;*/
        /*height: calc(100vh - 60px);*/
        /*height: calc(var(--vh, 1vh) * 100 - 60px) !important;*/
        /*overflow-y: auto;*/
        /*-webkit-overflow-scrolling: touch;*/
        /*background: white;*/
    /*}*/

    /*.main-header-container .navbar-collapse:before {*/
        /*display: none;*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon {*/
        /*-webkit-box-sizing: content-box;*/
        /*-moz-box-sizing: content-box;*/
        /*box-sizing: content-box;*/
        /*font-size: 2em;*/
        /*width: 42px;*/
        /*height: 60px;*/
        /*line-height: 60px;*/
        /*color: #000000;*/
        /*border-left: 1px solid transparent;*/
        /*border-right: 1px solid transparent;*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon:after,*/
    /*.main-header-container .main-navigation-search-icon:before {*/
        /*right: 0;*/
        /*margin: auto;*/
        /*bottom: 0;*/
        /*left: 0;*/
        /*top: 0;*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon.active {*/
        /*border-left: 1px solid #c2c3c6;*/
        /*border-right: 1px solid #c2c3c6;*/
        /*background-color: #efeff0;*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon.active:after,*/
    /*.main-header-container .main-navigation-search-icon.active:before {*/
        /*position: absolute;*/
        /*z-index: 1;*/
        /*display: block;*/
        /*width: 24px;*/
        /*height: 1px;*/
        /*border-radius: 2px;*/
        /*background: #000000;*/
        /*content: '';*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon.active:after {*/
        /*-webkit-transform: rotate(45deg);*/
        /*-ms-transform: rotate(45deg);*/
        /*-o-transform: rotate(45deg);*/
        /*transform: rotate(45deg);*/
    /*}*/

    /*.main-header-container .main-navigation-search-icon.active:before {*/
        /*-webkit-transform: rotate(-45deg);*/
        /*-ms-transform: rotate(-45deg);*/
        /*-o-transform: rotate(-45deg);*/
        /*transform: rotate(-45deg);*/
    /*}*/

    /*.main-header-container .navbar-toggle {*/
        /*margin: 0;*/
        /*order: 1;*/
        /*height: 60px;*/
        /*line-height: 60px;*/
        /*!*border-left: 1px solid #dddedf;*!*/
        /*background-color: white;*/
        /*padding: 0 10px;*/
        /*box-sizing: border-box;*/
        /*top: 1px;*/
    /*}*/

    /*.main-header-container .navbar-toggle.collapsed {*/
        /*border-color: transparent;*/
        /*height: 59px;*/
        /*top: 0;*/
    /*}*/

    /*.main-header-container .navbar-toggle .patty {*/
        /*-webkit-transition: all 0.2s ease;*/
        /*-o-transition: all 0.2s ease;*/
        /*transition: all 0.2s ease;*/
        /*top: -4px;*/
        /*position: relative;*/
        /*width: 24px;*/
        /*height: 1px;*/
        /*margin: 0;*/
        /*padding: 0;*/
        /*border-radius: 2px;*/
        /*display: inline-block;*/
        /*background: black;*/
    /*}*/

    /*.main-header-container .navbar-toggle .patty:after,*/
    /*.main-header-container .navbar-toggle .patty:before {*/
        /*-webkit-transition: all 0.2s ease;*/
        /*-o-transition: all 0.2s ease;*/
        /*transition: all 0.2s ease;*/
        /*position: absolute;*/
        /*z-index: 1;*/
        /*display: block;*/
        /*width: 24px;*/
        /*height: 1px;*/
        /*border-radius: 2px;*/
        /*background: black;*/
        /*content: '';*/
    /*}*/

    /*.main-header-container .navbar-toggle .patty:after {*/
        /*top: 6px;*/
    /*}*/

    /*.main-header-container .navbar-toggle .patty:before {*/
        /*top: -6px;*/
    /*}*/

    /*.main-header-container .navbar-toggle:not(.collapsed) .patty {*/
        /*background: none;*/
    /*}*/

    /*.main-header-container .navbar-toggle:not(.collapsed) .patty:before {*/
        /*-webkit-transform: rotate(-45deg);*/
        /*-ms-transform: rotate(-45deg);*/
        /*-o-transform: rotate(-45deg);*/
        /*transform: rotate(-45deg);*/
        /*top: 0;*/
    /*}*/

    /*.main-header-container .navbar-toggle:not(.collapsed) .patty:after {*/
        /*-webkit-transform: rotate(45deg);*/
        /*-ms-transform: rotate(45deg);*/
        /*-o-transform: rotate(45deg);*/
        /*transform: rotate(45deg);*/
        /*top: 0;*/
    /*}*/
/*}*/

/*@media (min-width: 641px) {*/
    /*.main-header-container .simple-responsive-banner-component {*/
        /*margin: 0;*/
    /*}*/

    /*.main-header-container .affix {*/
        /*width: 100%;*/
    /*}*/

    /*.main-navigation-mobile-header {*/
        /*margin-right: 40px;*/
    /*}*/

    /*.main-header-navigation {*/
        /*position: relative;*/
        /*margin: 0;*/
        /*min-width: 1260px;*/
        /*z-index: 1000;*/
        /*border-bottom: 1px solid #979797;*/
        /*transition: all .3s linear;*/
        /*background-color: white;*/
        /*top: 0;*/
        /*height: 60px;*/
        /*box-sizing: border-box;*/
        /*display: flex;*/
        /*align-items: center;*/
        /*width: 100%;*/
        /*padding-left: 20px;*/
        /*padding-right: 30px;*/
    /*}*/

    /*.main-header-navigation .navbar-collapse {*/
        /*display: flex !important;*/
        /*margin: 0;*/
        /*min-height: 0;*/
        /*border: none;*/
        /*position: static;*/
        /*flex: 1;*/
        /*padding: 0;*/
        /*justify-content: space-between;*/
    /*}*/

    /*.main-header-navigation .navbar-collapse:before {*/
        /*display: none;*/
    /*}*/

    /*.main-header-navigation .logo img {*/
        /*width: 105px;*/
        /*max-width: 105px;*/
    /*}*/
/*}*/

.wiley-cookie-location,
.wiley-session-location {
    font-weight: bold;
}

@media (min-width: 1240px) {
    .main-navigation-mobile-header {
        margin-right: 5%;
    }
}

@media (min-width: 641px) {
    .navigation-menu-items {
        margin: 0;
        padding: 0;
        list-style: none;
        display: flex;
        font-family: 'Open Sans', sans-serif;
        flex: 1;
        text-transform: uppercase;
        font-size: 1.6em;
    }

    .navigation-menu-items > li {
        display: inline-block;
        line-height: 60px;
        padding-right: 20px;
    }

    .navigation-menu-items > li.dropdown-submenu {
        position: relative;
    }

    .navigation-menu-items > li.dropdown-submenu:after {
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

    .navigation-menu-items > li.dropdown-submenu.hover:after {
        top: 29px;
        transform: rotate(-135deg);
    }

    .navigation-menu-items > li:last-child a {
        padding-right: 0;
    }

    .navigation-menu-items > li > a {
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

    .navigation-menu-items > li > a:hover,
    .navigation-menu-items > li > a:focus {
        text-decoration: none;
        outline: 0 solid transparent;
        color: #009ca9;
    }

    .navigation-menu-items > li > a.collapsed {
        position: relative;
        padding-right: 0;
    }

    .navigation-menu-items > li.hover .dropdown-menu {
        display: block;
        z-index: 1;
    }

    .navigation-menu-items > li.hover > a {
        color: #009ca9;
    }

    .navigation-menu-items > li:hover > a,
    .navigation-menu-items > li:focus > a {
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
        /*border: solid #c2c3c6;*/
        /*border-width: 0 1px 1px 0;*/
        display: inline-block;
        padding: 3px;
        transform: rotate(-45deg);
        -webkit-transform: rotate(-45deg);
    }
}
@media (max-width: 846px) {
    .navigation-menu-items {
        margin: 0;
        padding: 0;
        list-style: none;
        display: flex;
        font-family: 'Open Sans', sans-serif;
        flex: 1;
        text-transform: uppercase;
        font-size: 1.4em;
    }

    .navigation-menu-items > li {
        display: inline-block;
        line-height: 60px;
        padding-right: 20px;
    }

    .navigation-menu-items > li.dropdown-submenu {
        position: relative;
    }

    .navigation-menu-items > li.dropdown-submenu:after {
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

    .navigation-menu-items > li.dropdown-submenu.hover:after {
        top: 29px;
        transform: rotate(-135deg);
    }

    .navigation-menu-items > li:last-child a {
        padding-right: 0;
    }

    .navigation-menu-items > li > a {
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

    .navigation-menu-items > li > a:hover,
    .navigation-menu-items > li > a:focus {
        text-decoration: none;
        outline: 0 solid transparent;
        color: #009ca9;
    }

    .navigation-menu-items > li > a.collapsed {
        position: relative;
        padding-right: 0;
    }

    .navigation-menu-items > li.hover .dropdown-menu {
        display: block;
        z-index: 1;
    }

    .navigation-menu-items > li.hover > a {
        color: #009ca9;
    }

    .navigation-menu-items > li:hover > a,
    .navigation-menu-items > li:focus > a {
        color: #009ca9;
    }

}

.main-navigation-menu.tablet .dropdown-menu .dropdown-items {
    width: 100%;
}

.main-navigation-menu.tablet .dropdown-menu .dropdown-items .dropdown-item {
    padding-right: calc(100% - 244px);
}

.main-navigation-menu.tablet .dropdown-menu .dropdown-items .dropdown-item.dropdown-submenu.three-levels > .dropdown-items-wrapper > .dropdown-items {
    width: 100%;
}

.main-navigation-menu.tablet .dropdown-menu .dropdown-items .dropdown-item.dropdown-submenu.three-levels > .dropdown-items-wrapper > .dropdown-items > .dropdown-item {
    padding-right: calc(100% - 275px);
}

@media (max-width: 640px) {
    .main-header-container .navigation-menu-items {
        padding: 20px 0;
        margin: 0;
    }

    .main-header-container .navigation-menu-items > li {
        list-style: none;
        margin: 0;
        position: relative;
        overflow: hidden;
        display: block;
        padding: 15px 30px 15px 15px;
    }

    .main-header-container .navigation-menu-items > li.dropdown-submenu:after {
        position: absolute;
        width: 0;
        content: '';
        height: 0;
        top: 35%;
        right: 20px;
        border: solid #1b1c1d;
        border-width: 0 1px 1px 0;
        display: inline-block;
        padding: 4px;
        transform: rotate(-45deg);
    }

    .main-header-container .navigation-menu-items > li > a {
        color: rgba(0, 0, 0, 0.87);
        background: none;
        font-weight: 600;
        font-size: 1.7em;
        text-decoration: none;
        line-height: 14px;
        text-transform: uppercase;
    }

    .main-header-container .navigation-menu-items .toggle-dropdown {
        right: 15px;
        position: absolute;
        top: 3px;
        margin: auto;
        width: 30px;
        padding: 0 20px;
        box-sizing: border-box;
    }

    .main-header-container .navigation-menu-items .toggle-dropdown:after {
        position: absolute;
        width: 0;
        content: '';
        height: 0;
        top: 15px;
        right: 20px;
        /*border: solid #1b1c1d;*/
        /*border-width: 0 1px 1px 0;*/
        display: inline-block;
        padding: 4px;
        transform: rotate(-45deg);
        -webkit-transform: rotate(-45deg);
    }

}

/*.main-header-container .main-navigation-search .input-group-btn button.glyphicon-search {*/
    /*top: 0;*/
/*}*/

/*.main-header-container .main-navigation-search .input-group-btn button.glyphicon-search:before {*/
    /*display: none;*/
/*}*/

/*@media (max-width:640px) {*/
    /*.main-header-container .main-navigation-search .input-group-btn {*/
        /*display: table-cell;*/
    /*}*/

    /*span.input-group-btn button {*/
        /*font-size: 0 !important;*/
    /*}*/

    /*.input-group-btn button.glyphicon-search:before {*/
        /*font-size: 26px !important;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .input-group-btn button {*/
        /*padding: 0 0;*/
        /*width: 55px;*/
    /*}*/

    /*.main-header-container .input-group-btn button.glyphicon-search {*/
        /*margin-top: -1px;*/
        /*border-radius: 3px;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group .main-navigation-search-input {*/
        /*border-radius: 3px;*/
        /*width: 98%;*/
        /*box-shadow: none;*/
    /*}*/

    /*.main-header-container .main-navigation-search .input-group-btn button.glyphicon-search:before {*/
        /*display: block;*/
    /*}*/

/*}*/


/*@media (min-width:641px) {*/

    /*.input-group-btn button.glyphicon-search {*/
        /*font-family: "Open Sans", "sans-serif" !important;*/
        /*font-size: 18px;*/
        /*line-height: 25px;*/
    /*}*/

/*}*/

</style>
