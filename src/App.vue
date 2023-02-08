<template>
<div id="app">
  
<contenu></contenu>
</div>
  
  
</template>

<script>

import Contenu from './components/ContenuDisplay.vue'

export default {
  name: 'App',
  components: {
   'contenu': Contenu
  }
}
</script>

<style>

</style>
