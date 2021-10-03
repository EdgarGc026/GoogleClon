<template>
  <section class="button-section">
    <div class="button-container">
      <button>Search with google</button>
      <button>I feel lucky</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "px-button",
};
</script>

<style>
.button-section {
  width: 530px;
  margin: 0 auto;
}

.button-container {
  display: inline-block;
}

.button-container button {
  height: 40px;
  background-color: #e8eaed;
  border: 0;
  font-size: 14px;
  font: #3c69ae;
  border-radius: 5px;
  padding: 0 15px;
  margin-right: 15px;
}

.button-container button:hover {
  cursor: pointer;
  border: 1px solid #c6c6c6;
  box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.1);
  color: #222;
  background-color: #f8f8f8;
  background-image: -webkit-linear-gradient(top, #f8f8f8, #f1f1f1);
}
</style>
