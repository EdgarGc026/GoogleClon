<template>
  <footer class="footer">
    <ul class="footer-left">
      <li><a href="#">Advertisting</a></li>
      <li><a href="#">Business</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">How Search Works</a></li>
    </ul>

    <ul class="footer-right">
      <li><a href="#">Privacy</a></li>
      <li><a href="#">Terms</a></li>
      <li><a href="#">Settings</a></li>
    </ul>
  </footer>
</template>

<script>
export default {
  name: "px-footer",
};
</script>

<style>
.footer {
  width: 100%;
  height: auto;
  position: absolute;
  bottom: 0;

  /* Using Grid property */
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  font-size: 13px;
  background-color: #f2f2f2;
  border-top: 1px solid #e4e4e4;
}

.footer ul {
  display: flex;
  margin: 10px;
  padding-left: 0px;
  list-style: none;
  text-decoration: none;
}

.footer .footer-left {
  justify-self: left;
}

.footer .footer-right {
  justify-self: right;
}

.footer ul li a {
  margin: 10px;
  color: #6f6f6f;
}
</style>
