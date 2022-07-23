<template>
  <div>
    <p class="overview">Overview - Today</p>
  </div>
</template>

<script>
export default {
  name: 'Overview',
  props: {
    msg: Number
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');
.overview{
  color:  hsl(0, 0%, 100%);
  font-family: 'Inter', sans-serif;
  font-size: 20px;
  font-weight: 700;
  padding: 20px 0px 0px 60px;
  margin-bottom: 15px;
  line-height: 0px;
}

</style>
