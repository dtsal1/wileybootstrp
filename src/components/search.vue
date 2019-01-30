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
                <ul id="ui-id-1" tabindex="0" class="ui-menu ui-widget ui-widget-content ui-autocomplete ui-front" style="display: none;">

                </ul>
            </form>

        </div>
    </div>
</template>

<script>
    export default {
        name: "search"
    }
</script>

<style scoped>

</style>