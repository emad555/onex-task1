<template>
  <div style="background-color: hsl(230, 17%, 14%);">

  <Title msg = "20" style="background-color: hsl(230, 17%, 14%);"/>

  <Platforms style="background-color: hsl(230, 17%, 14%);"/>
  <Overview style="background-color: hsl(230, 17%, 14%);"/>
  <Actions style="background-color: hsl(230, 17%, 14%);"/>
  
</div>


</template>

<script>
import Title from './components/Title.vue'
import Overview from './components/Overview.vue'
import Platforms from './components/Platforms.vue'
import Actions from './components/Actions.vue'

export default {
  name: 'App',
  components: {
    Title,
    Platforms,
    Overview,
    Actions
  }
}
</script>

<style>
*{
  

}
</style>
