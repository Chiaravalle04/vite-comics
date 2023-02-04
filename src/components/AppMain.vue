<script>
import AppCard from './AppCard.vue'

export default {
  name: 'AppMain',

  components: {
    AppCard
  },
  
  data() {
  
    return {

    }
  }
}
</script>

<template>

  <main>

    <div class="container">

      <div class="general-container">

        <div class="title-container">
          <p>CURRENT SERIES</p>
        </div>

        <AppCard/>

        <button>LOAD MORE</button>

      </div>

    </div>


  </main>
    
</template>

<style lang="scss" scoped>
main {
    padding-top: 350px;
    min-height: 350px;
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: contain;
    .container {
      background-color: #1c1c1c;
      position: relative;
      .title-container {
        width: 250px;
        height: 50px;
        background-color: #0383f9;
        position: absolute;
        top: -25px;
        p {
          color: #fff;
          font-weight: bold;
          font-size: 20px;
          text-align: center;
          line-height: 50px;
        }
      }
      .general-container {
        padding: 40px 0;
        background-color: #1c1c1c;
        button {
          display: block;
          width: 200px;
          height: 40px;
          margin: 0 auto;
          background-color: #0383f9;
          color: #fff;
          border: 0;
          font-weight: bold;
          cursor: pointer;
        }
      }
    }
  
}   
</style>