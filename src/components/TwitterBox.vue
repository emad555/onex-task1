<template>
  <div class="flexbox-item"></div>
</template>

<script>

export default {
  name: 'TwitterBox',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');
.flexbox-item{
  width: 200px;
  margin: 10px;
  border: 3px solid #333;
  background-color: hsl(228, 28%, 20%);
  min-height: 180px;
  padding: 0px 0px 0px 0px;
  border-radius: 5px;
  border-top: 3px solid hsl(203, 89%, 53%);
}

</style>
