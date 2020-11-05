<template>
  <div class="gallery">
    <img class="gallery__image gallery__image--photo1" src="../../assets/img/photo1.png" />
    <img class="gallery__image gallery__image--photo2" src="../../assets/img/photo2.png" />
    <img class="gallery__image gallery__image--photo3" src="../../assets/img/photo3.png" />
    <img class="gallery__image gallery__image--photo4" src="../../assets/img/photo4.png" />
    <img class="gallery__image gallery__image--photo5" src="../../assets/img/photo5.png" />
    <img class="gallery__image gallery__image--photo6" src="../../assets/img/photo6.png" />
  </div>
</template>

<script>
export default {
  name: "Gallery",
};
</script>

<style>
.gallery {
  width: 95%;
  margin: 7% auto;
  display: grid;
  grid-template-rows: 33.33%;
  grid-template-rows: auto;
  grid-template-areas:
    "photo1 photo2 photo2"
    "photo3 photo3 photo4"
    "photo5 photo6 photo4"
}

.gallery__image {
  width: 100%;
  border-radius: 20px;
  padding: 5px;
  filter: drop-shadow(0px 4px 6px rgba(0, 0, 0, 0.15));
}

.gallery__image--photo1{
  height: 110px;
  
  grid-area: photo1;

}
.gallery__image--photo2{
  height: 110px;
  grid-area: photo2;

}
.gallery__image--photo3{
  height: 110px;
  grid-area: photo3;
}
.gallery__image--photo4{
  height: 225px;
  grid-area: photo4;

}
.gallery__image--photo5{
  height: 110px;
  grid-area: photo5;

}
.gallery__image--photo6{
  height: 110px;
  grid-area: photo6;
}

</style>
