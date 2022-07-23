<template>

<div class="parent">  
  <div class="flexbox-item" :style="line">
      <div class="flex" style="align-items: center; padding-top: 22px; padding-right: 20px;">
        <div class="text">
          {{extn}}
        </div>
        
        <div class="png" style="margin-left: 65px">
          <img :src="require(`@/images/${link}`)"> 
        </div>
        

        
      </div>

      <div class="numbers flex" style="align-items: left; padding-top: 10px;">
        {{numbers}}
          <div class="today" :style="color" style="align-items: center; padding-top: 10px; margin-left: 55px;">
         <img :src="require(`@/images/${arrow}`)"> 
        {{daily}}%  
      </div>
      </div>

</div>


    
      


  </div>
</template>

<script>

export default {
  name: 'Statistics',
  props: [
    "link",
    "extn",
    "numbers",
    "daily",
    "arrow",
    "line",
    "color"

  ],
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap');

.parent {
  display: flex;
  flex-wrap: wrap;
}



.flexbox-item{
  width: 200px;
  margin: 10px;
  background-color: hsl(228, 28%, 20%);
  min-height: 100px;
  border-radius: 5px;
  cursor: pointer;
  
}


.flex{
  background-color: hsl(228, 28%, 20%);
  display: flex;  
  justify-content: center;  
}

.icon{
width:"30"; 
height:"30";
background-color: hsl(228, 28%, 20%);
}

.text{
background-color: hsl(228, 28%, 20%);
color: hsl(228, 34%, 66%);
font-family: 'Inter', sans-serif;
font-size: 12px;
}

.numbers{
background-color: hsl(228, 28%, 20%);
color: white;
font-weight: bold;
font-family: 'Inter', sans-serif;
font-size: 25px;
justify-content: left;
padding-left: 15px;
}



.today{
font-family: 'Inter', sans-serif;
font-size: 11px;
font-weight:bold;
background-color: hsl(228, 28%, 20%);
display: flex;  
justify-content: center;
padding-left: 20px;
}


</style>
