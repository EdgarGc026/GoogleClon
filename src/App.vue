<template>
  <div id="app">
    <px-header :avatarUrl="avatarUrl" :avatarName="avatarName" />

    <main>
      <px-logo :logoImg="logoImg" :logoName="logoName" />
      <px-input />
      <px-button />
    </main>
    <px-footer />
  </div>
</template>

<script>
import PxButton from "./components/PxButton.vue";
import PxFooter from "./components/PxFooter.vue";
import PxHeader from "./components/PxHeader.vue";
import PxInput from "./components/PxInput.vue";
import PxLogo from "./components/PxLogo.vue";

export default {
  name: "App",

  data() {
    return {
      avatarName: "EdgarGc picture",
      avatarUrl:
        "https://lh3.googleusercontent.com/ogw/ADGmqu_FkrxOhCqb8uYNYuN34_kJ-tpDigEPqIDsk-r3eg=s32-c-mo",
      logoImg: require("./assets/logo-google.png"),
      logoName: "Main Google logo",
    };
  },

  components: {
    PxHeader,
    PxLogo,
    PxInput,
    PxButton,
    PxFooter,
  },
};
</script>

<style>
body {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-size: 13px;
  font-family: Arial, Helvetica, sans-serif;
}

a {
  text-decoration: none;
  cursor: pointer;
}

main {
  margin-top: 150px;
  text-align: center;
}
</style>
