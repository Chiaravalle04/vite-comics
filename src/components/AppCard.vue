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
      <img :src="thumb" :alt="title">
      <p class="title">{{ title }}</p>
      <p class="feature"> <b>Price:</b> {{ price }}</p>
      <p class="feature"> <b>Type:</b> {{ type }}</p>
      <button id="buy"><i class="fa-solid fa-cart-shopping fa-lg"></i></button>
  </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/varcolor.scss' as *;

img {
  width: 100%;
}
.title {
    text-transform: uppercase;
    font-weight: bold;
    padding-top: 10px;
    color: $secondColor;
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
  background-color: $mainColor;
  color: $secondColor;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  cursor: pointer;
}
</style>
