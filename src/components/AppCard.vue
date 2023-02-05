<script>
export default {
  name: 'AppCard',
  props: {
    thumb: String,
    title: String,
    price: String,
    type: String
  },
  
  data() {
  
    return {
        
    }
  }
}
</script>

<template>
    
  <div>
      <img :src="thumb" alt="">
      <p class="title">{{ title }}</p>
      <p class="feature"> <b>Price:</b> {{ price }}</p>
      <p class="feature"> <b>Type:</b> {{ type }}</p>
      <button id="buy"><i class="fa-solid fa-cart-shopping fa-lg"></i></button>
  </div>

</template>

<style lang="scss" scoped>
img {
  width: 100%;
}
.title {
    text-transform: uppercase;
    font-weight: bold;
    padding-top: 10px;
    color: #f4ece2;
}
.feature {
    color: #787879;
    padding: 5px 0;
    text-transform: capitalize;
}
#buy {
  display: block;
  width: 50%;
  margin: 0 auto;
  line-height: 40px;
  border: 0;
  background-color: #0383f9;
  color: #fff;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  cursor: pointer;
}
</style>
