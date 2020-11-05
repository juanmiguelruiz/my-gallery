<template>
  <div class="container">
    <div class="row">
      <div class="col-12 d-flex justify-content-center profile">
        <img
          :src="require(`@/assets/img/${photo}.png`)"
          class="profile__image"
          alt="..."
        />
      </div>
      <div class="col-12 d-flex justify-content-center ">
        <p class="profile__name">{{ name }}</p>
      </div>
      <div class="col-12 d-flex justify-content-center ">
        <p class="profile__location">{{ location }}</p>
      </div>
      <div class="profile__stats">
        <div class="profile__stats--posts"><Stat name="Posts" number="100" /></div>
        <div class="profile__stats--followers"><Stat name="Followers" number="2.242" /></div>
        <div class="profile__stats--following"><Stat name="Following" number="1,432" /></div>
      </div>
    </div>
  </div>
</template>

<script>
import Stat from "../Stat";

export default {
  name: "Profile",
  components: {
    Stat,
  },
  props: {
    name: {
      type: String,
      required: true,
      default: "",
    },
    location: {
      type: String,
      required: true,
      default: "",
    },
    photo: {
      type: String,
      required: true,
    },
  },
};
</script>

<style src="./styles.css" />
