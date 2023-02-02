<script>
export default {
  name: 'AppMain',
  
  data() {
  
    return {
  
    }
  }
}
</script>

<template>

  <main>

    <div class="main-container">
      <p>Content goes here</p> 
    </div>

  </main>
    
</template>

<style lang="scss" scoped>
main {
  background-color: black;
  min-height: 100px;
  .main-container {
    width: 80%;
    margin: 0 auto;
    p {
      color: #fff;
      line-height: 100px;
    }
  }
}   
</style>