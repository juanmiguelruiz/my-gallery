<template>
  <div id="app">
    <Profile
      name="Rodney Cotton"
      location="Helsinki, Finland"
      photo="profilePhoto"
    />
    <Gallery />
    <footer class="my-gallery__footer">juanmiguelruiz@ DevChallenges.io</footer>
  </div>
</template>

<script>
import Vue from "vue";
import Bootstrap from "./components/Bootstrap";
import Profile from "./components/Profile";
import Gallery from "./components/Gallery";

Vue.use(Bootstrap);

export default {
  name: "App",
  components: {
    Profile,
    Gallery,
  },
};
</script>

<style>
@import url(
  https://fonts.googleapis.com/css?family=Montserrat:100,
  200,
  300,
  400,
  500,
  600,
  700,
  800,
  900
);

.selector-for-some-widget {
  box-sizing: content-box;
}

.my-gallery__footer {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 17px;
  color: #a9a9a9;
  text-align: center;
  padding: 5% 0;
}

/*Tablet*/

@media screen and (min-width: 768px) and (max-width: 1023px) {
  .my-gallery__footer {
    font-size: 16px;
  }
}

/*Laptop L*/

@media screen and (min-width: 1440px) {
    .my-gallery__footer {
    font-size: 17px;
  }
}
</style>
