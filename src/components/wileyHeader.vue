<template>
    <header id="main-header-container" class="main-header-container">
        <div class="main-sticky-header affix-top">
            <div class="main-header-navigation">
                <div class="main-navigation-mobile-header">
                    <div class="yCmsContentSlot logo">
                        <div class="simple-responsive-banner-component">
                            <a href="https://www.wiley.com/en-gb/">
                                <img class="js-responsive-image" alt="Wiley" title="Wiley" style="" src="../assets/b2c-site-logo_desktop_optimized.png">
                            </a>
                        </div>
                    </div>
                    <span type="button" class="navbar-toggle collapsed visible-xs-inline-block">
                             <span class="patty"></span>
                          </span>
                    <span class="main-navigation-search-icon icon-search-black visible-xs-inline-block"></span>

                </div>
                <nav id="main-header-navbar" role="navigation" class="collapse navbar-collapse navbar">
                    <ul class="navigation-menu-items initialized">
                        <li class=""><a href="" class="collapsed">{{msgProducts}}</a>
                        </li>
                        <li class=""><a href="" class="collapsed">{{msgWork}}</a>
                        </li>
                        <li class=""><a href="" class="collapsed">{{msgCompany}}</a>
                        </li>
                        <li class=""><a href="" class="collapsed">{{msgContact}}</a>
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
        }
    }
</script>

<style scoped>

</style>