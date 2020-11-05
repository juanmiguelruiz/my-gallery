<template>
  <div class="profile__stat">
    <p class="profile__stat__text">{{number}}</p>
    <p class="profile__stat__text">{{name}}</p>
  </div>
</template>

<script>
export default {
  name: "Stat",
  props: {
    name: {
      type: String,
      required: true,
      default: "",
    },
    number: {
      type: String,
      required: true,
      default: "",
    },
  },
};
</script>

<style/>
