<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const tshirt = ref('')

</script>
<template>
  <div  class="container-md ">
  <div class="text-bg-info p-3">
<h2>    Available T-shirts</h2>
    <select v-model="tshirt" class="form-select" aria-label="Default select example">
        <option value="ClassicCotton Creations">ClassicCotton Creations</option>
        <option value="AdventureWear">AdventureWear</option>
        <option value="ColorSplash Tees">ColorSplash Tees</option>
        <option value="ProFlex Athletic Gear">ProFlex Athletic Gear</option>
        <option value="ComfyKids Creations">ComfyKids Creations</option>
        <option value="ArtisticExpress Tees">ArtisticExpress Tees</option>
        
    </select>
    <p v-if="tshirt == 'ClassicCotton Creations'">
      <h3>ClassicCotton Creations</h3>
<strong>Size:</strong> Available in XS to 4XL, offering a comfortable fit for everyone.<br>
<strong>Made From:</strong> Our t-shirts are expertly crafted with 100% organic cotton.<br>
<strong>Established:</strong> ClassicCotton Creations, delivering timeless style, since 2010.

    </p>
    <p v-if="tshirt == 'AdventureWear'">
      <h3>AdventureWear</h3>
<strong>Size:</strong> Our t-shirts come in sizes from S to 3XL, perfect for outdoor enthusiasts.<br>
<strong>Made From:</strong> Designed with a quick-drying blend of polyester and spandex for ultimate comfort on your adventures.<br>
<strong>Established:</strong> AdventureWear, your companion for outdoor journeys, since 2013.

</p>
<p v-if="tshirt == 'ColorSplash Tees'">
  <h3>ColorSplash Tees</h3>
<strong>Size:</strong> Available in XS to XXL, providing a colorful fit for all.<br>
<strong>Made From:</strong> Our t-shirts are made from 100% ring-spun combed cotton, offering vibrant colors and softness.<br>
<strong>Established:</strong> ColorSplash Tees, adding a splash of color to your wardrobe, since 2015.

</p>
<p v-if="tshirt == 'ProFlex Athletic Gear'">
  <h3>ProFlex Athletic Gear</h3>
<strong>Size:</strong> Our athletic t-shirts are available in sizes from XS to 4XL, ensuring maximum flexibility and comfort.<br>
<strong>Made From:</strong> Crafted with advanced moisture-wicking fabric to enhance your athletic performance.<br>
<strong>Established:</strong> ProFlex Athletic Gear, powering your workouts, since 2016.

</p>
<p v-if="tshirt == 'ComfyKids Creations'">
  <h3>ComfyKids Creations</h3>
<strong>Size:</strong> Our kids' t-shirts come in sizes from 2T to 14T, making sure your little ones are cozy and stylish.<br>
<strong>Made From:</strong> Designed with soft and durable materials, perfect for active play and everyday wear.<br>
<strong>Established:</strong> ComfyKids Creations, keeping kids comfy and happy, since 2014.

</p>
<p v-if="tshirt == 'ArtisticExpress Tees'">
  <h3>ArtisticExpress Tees</h3>
<strong>Size:</strong> Available in sizes from XS to XL, bringing artistic expression to all.<br>
<strong>Made From:</strong> Our t-shirts are made from a blend of organic cotton and recycled polyester, combining creativity with sustainability.<br>
<strong>Established:</strong> ArtisticExpress Tees, making fashion a canvas for art, since 2011.

</p>
</div>
  </div>

</template>