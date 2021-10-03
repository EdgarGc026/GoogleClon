<template>
  <section class="input-section">
    <div class="input-container">
      <span class="input-search-icon"></span>
      <input type="text" />
      <a href="#" class="input-micro-icon"></a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.input-section {
  width: 530px;
  margin: 0 auto;
  margin-bottom: 35px;
}

.input-container {
  width: 525px;
  border-radius: 100px;
  border: 1px solid #dfe1e5;
  display: flex;
  justify-content: center;
  align-items: center;
}

.input-container input {
  width: 450px;
  height: 43px;
  border: none;
  outline: none;
}

.input-container:hover {
  box-shadow: 0px 1px 6px 0px #20212447;
  border-color: #dfe1e500;
}
.input-container .input-search-icon {
  width: 18px;
  height: 18px;
  margin-right: 10px;
  background-image: url("https://img.icons8.com/android/24/000000/search.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}

.input-container .input-micro-icon {
  width: 20px;
  height: 20px;
  background-image: url("https://www.gstatic.com/images/branding/googlemic/2x/googlemic_color_24dp.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}
</style>
