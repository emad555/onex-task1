<template>

  <div class="flexbox-item" :style="line">
      <div class="flex" style="align-items: center; padding-top: 22px;">
        
        <div class="png" style="margin-right: 4px">
          <img :src="require(`@/images/${link}`)"> 
        </div>
        
        <div class="text">
          {{extn}}
        </div>
        
      </div>

      <div class="numbers flex" style="align-items: center; padding-top: 10px;">
        {{numbers}}
      </div>

      <div class="followers flex" style="align-items: center; padding-top: 5px;">
         FOLLOWERS
      </div>

      <div class="today" style="align-items: center; padding-top: 10px;">
         <img :src="require(`@/images/${arrow}`)"> 
        {{daily}}%  Today 
      </div>
      


  </div>
</template>

<script>

export default {
  name: 'Box',
  props: [
    "link",
    "extn",
    "numbers",
    "daily",
    "arrow",
    "line"

  ],
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap');
.flexbox-item{
  width: 200px;
  margin: 10px;
  background-color: hsl(228, 28%, 20%);
  min-height: 180px;
  border-radius: 5px; 
   cursor: pointer; 
}


.flex{
  display: flex;  
  justify-content: center;
    
}

.icon{
width:"30"; 
height:"30";
background-color: hsl(228, 28%, 20%);
}

.text{
color: hsl(228, 34%, 66%);
font-family: 'Inter', sans-serif;
font-size: 12px;
}

.numbers{
color: white;
font-weight: bold;
font-family: 'Inter', sans-serif;
font-size: 35px;
justify-content: center;

}

.followers{
letter-spacing: 4px;
font-family: 'Inter', sans-serif;
color: hsl(228, 34%, 66%);
font-size: 11px;
}

.today{
font-family: 'Inter', sans-serif;
color: hsl(163, 72%, 41%);
font-size: 11px;
font-weight:bold;
display: flex;  
justify-content: center;
}

.flexbox-item:hover {
  background-color: hsl(228, 20%, 29%);
  z-index: -1; 
}




</style>
