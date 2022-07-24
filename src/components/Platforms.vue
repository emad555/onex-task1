<template>
  <div class="flexbox-container">
    <div v-for="(item) in socials" :key="item" style="color:white">
    <box
      :link="item.link"
      :extn="item.ext"
      :numbers="item.numbers"
      :daily="item.inc"
      :arrow="item.arrow"
      :line="item.line"
    ></box>
   
    </div>
  </div>
</template>
<script>
import Box from "./Box.vue";
import IgBox from "./IgBox.vue";
/* import TwitterBox from './TwitterBox.vue'
import IgBox from './IgBox.vue'
import YoutubeBox from './YoutubeBox.vue' */
export default {
  name: "Platforms",
  props: {
    msg: String,
  },
  components: {
    Box,
    IgBox
},

  data() {
    return {
      test: null,
      socials: [
        {
          link: "icon-facebook.svg",
          ext: "@nathanf",
          numbers: 1987,
          inc: 20,
          arrow: "icon-up.svg",
          line: "border-top: 3px solid hsl(208, 92%, 53%);",
          id: 1,
        },
        {
          link: "icon-twitter.svg",
          ext: "@nathanf",
          numbers: 1044,
          inc: 99,
          arrow: "icon-up.svg",
          line: "border-top: 3px solid hsl(203, 89%, 53%);",
          id: 2,
        },
        {
          link: "icon-instagram.svg",
          ext: "@reelnathanf",
          numbers: 11000,
          inc: 1099,
          arrow: "icon-up.svg",
          line:"border-top: 1rem solid;border-width: 3px;border-image: linear-gradient(90deg, hsl(37, 97%, 70%) ,hsl(329, 70%, 58%)) 2;",
          id: 3,
        },
        {
          link: "icon-youtube.svg",
          ext: "@Nathan F.",
          numbers: 8239,
          inc: 144,
          arrow: "icon-up.svg",
          line: "border-top: 3px solid  hsl(348, 97%, 39%);",
          id: 4,
        },
        
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter&display=swap");
.flexbox-container {
  display: flex;
    padding: 0px 0px 0px 50px;
    flex-wrap: wrap;
}
</style>
