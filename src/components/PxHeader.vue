<template>
  <header class="header">
    <nav class="navbar">
      <ul class="menu-right">
        <li class="menu-item">
          <a target="_blank" :href="gmailUrl">Gmail</a>
        </li>
        <li class="menu-item">
          <a target="_blank" :href="imagesUrl">Images</a>
        </li>
        <li class="menu-icon">
          <a href="#"></a>
        </li>
        <li class="menu-item">
          <a href="#">
            <img :src="avatarUrl" :alt="avatarName" />
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "px-header",
  props: {
    avatarUrl: { type: String, required: true },
    avatarName: { type: String, required: true },
  },
  data() {
    return {
      gmailUrl: "https://mail.google.com",
      imagesUrl: "https://www.google.com.mx/imghp",
    };
  },
};
</script>

<style>
a {
  text-decoration: none;
  cursor: pointer;
}

.header {
  width: 100%;
  height: 60px;
}

.navbar {
  display: flex;
  justify-content: flex-end;
}

.menu-right {
  width: 250px;
  height: auto;

  display: flex;
  list-style: none;
  justify-content: center;
  align-items: center;
}

.menu-item a {
  margin-right: 15px;
  color: #000000;
}

.menu-right .menu-icon {
  width: 25px;
  height: 25px;
  background-image: url("https://static.thenounproject.com/png/756729-200.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}

.menu-item a img {
  border-radius: 50%;
  margin-left: 10px;
}
</style>
