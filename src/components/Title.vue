<template>
  <div class="flex-container">
    <div>
    <p class="title">Social Media Dashboard</p>
    <p class="total-followers"> Total followers = {{msg}}</p>
    </div>
    <div>
      <Switch class="switch"/>
    </div>
  </div>
</template>

<script>

import Switch from '../components/Switch.vue'

export default {
  name: 'Title',
    components: {
    Switch
    }
    ,
  props: {
    msg: Number
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');

.title{
  color:  hsl(0, 0%, 100%);
  font-family: 'Inter', sans-serif;
  font-size: 20px;
  font-weight: 700;
  padding: 20px 0px 0px 60px;
  margin-bottom: 15px;
  line-height: 0px;
  
}
.total-followers{
  color:  hsl(228, 34%, 66%);
  font-family: 'Inter', sans-serif;
  font-size: 10px;
  font-weight: 400;
  padding: 0px 0px 0px 60px;


}

.flex-container {
  display: flex;
  flex-wrap: nowrap;
}

.switch{
  padding-top: 30px;
  position: absolute;
  top: 0px;
  right: 10px;
}



</style>
