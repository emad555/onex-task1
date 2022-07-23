<template>
  <div class="flexbox-container">
    <div v-for="(item) in action" :key="item" style="color:white">
    <statistics
      :link="item.link"
      :extn="item.ext"
      :numbers="item.numbers"
      :daily="item.inc"
      :arrow="item.arrow"
      :line="item.line"
      :color="item.color"
    ></statistics>
   
    </div>
  </div>
</template>
<script>
import Statistics from "./Statistics.vue";
/* import TwitterBox from './TwitterBox.vue'
import IgBox from './IgBox.vue'
import YoutubeBox from './YoutubeBox.vue' */
export default {
  name: "Actions",
  props: {
    msg: String,
  },
  components: {
    Statistics
},

  data() {
    return {
      test: null,
      action: [
        {
          link: "icon-facebook.svg",
          ext: "Page Views",
          numbers: 870,
          inc: 3,
          arrow: "icon-up.svg",
          color: "color:hsl(163, 72%, 41%);",
          id: 1,
        },
        {
          link: "icon-facebook.svg",
          ext: "Likes",
          numbers: 5200,
          inc: 2,
          arrow: "icon-down.svg",
          color: "color:red",
          id: 2,
        },
        {
          link: "icon-instagram.svg",
          ext: "Likes",
          numbers: 5462,
          inc: 2257,
          arrow: "icon-up.svg",
          color:"color:hsl(163, 72%, 41%);",
          id: 3,
        },
        {
          link: "icon-instagram.svg",
          ext: "Profile Views",
          numbers: 52,
          inc: 1375,
          arrow: "icon-up.svg",
          color:"color:hsl(163, 72%, 41%);",
          id: 4,
        },
        {
          link: "icon-twitter.svg",
          ext: "retweets",
          numbers: 117,
          inc: 303,
          arrow: "icon-up.svg",
          color:"color:hsl(163, 72%, 41%);",
          id: 5,
        },
                {
          link: "icon-twitter.svg",
          ext: "Likes",
          numbers: 8239,
          inc: 144,
          arrow: "icon-up.svg",
          color:"color:hsl(163, 72%, 41%);",
          id: 5,
        },
                {
          link: "icon-youtube.svg",
          ext: "Likes",
          numbers: 107,
          inc: 19,
          arrow: "icon-down.svg",
          color:"color:red",
          id: 5,
        },
                {
          link: "icon-youtube.svg",
          ext: "Total Views",
          numbers: 1407,
          inc: 12,
          arrow: "icon-down.svg",
          color:"color:red",
          id: 5,
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
