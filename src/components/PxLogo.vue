<template>
  <section class="logo-section">
    <img :src="logoImg" :alt="logoName" />
  </section>
</template>

<script>
export default {
  name: "px-logo",
  props: {
    logoImg: {
      type: String,
      required: true,
    },
    logoName: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.logo-section {
  width: 530px;
  margin: 0 auto;
  margin-bottom: 35px;
}

.logo-section img {
  width: 300px;
}
</style>
