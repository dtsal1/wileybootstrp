<template>
    <div class = 'slides'>
        <div v-bind.style="{ width: innerWidth +'px' }" class = 'slides-inner'>
            <app-slide v-for = "(Slide,index) in slides" v-bind:style="{width: singleWidth+'px', display: displaySlide[index]}" v-bind:oneSlide="Slide">
            </app-slide>
        </div>
        <div class="navigation">
            <span id = "prev" v-on:click="goTo">Prev</span>
            <span class = "nav_number" v-for="(i,index) in slides" v-on:click="goTo">{{index+1}} </span>
            <span id = "next" v-on:click="goTo">Next</span>
        </div>
    </div>
</template>

<script>
    import oneSlide from './oneSlide.vue'
    export default {
        name: "slides",
        data() {
            return {
                slides: [
                    { src: "./src/assets/Telescope_desktop.jpg"},
                    { src: "./src/assets/telescopeDesert.jpg"},
                    { src: "./src/assets/treesDesert.jpg"},
                    { src: "./src/assets/starSky.jpg"}
                ],

                innerWidth: 0,
                singleWidth:0,
                i:0,
                j:0,
                displaySlide: ['inline-block','none','none','none']
            }
        },
        components: {
            appSlide: oneSlide
        },

        props: {
          itemsPerSlide:{
              type: null,
              default: 1
          }
        },

        methods: {
            goTo(a)
            {
              console.log('печатаем хрень')
                // if (e != undefined) {
                  switch (a) {
                      case 1: {
                          this.displaySlide = ['inline-block', 'none', 'none', 'none'];
                          break;
                      }
                      case 2: {
                          this.displaySlide = ['none', 'inline-block', 'none', 'none'];
                          break;
                      }
                      case 3: {
                          this.displaySlide = ['none', 'none', 'inline-block', 'none'];
                          break;
                      }
                      case 4: {
                          this.displaySlide = ['none', 'none', 'none', 'inline-block'];
                          break;
                      }
                  // }


              }
            },
            Person (a) {
            setInterval(() => {

              this.goTo(a);
              if (a == 4) {
                  a = 0}
              a++;
            }, 3000)
    }

        },
        mounted () {
            window.onload = (event) => {
                this.singleWidth = this.$el.clientWidth;
            },
            window.onresize = (event) => {
                this.singleWidth = this.$el.clientWidth / this.itemsPerSlide;
                this.innerWidth = this.singleWidth * this.slides.length;
            }
            this.goTo();
            this.Person(this.j);

        }



    }
</script>

<style scoped>

</style>