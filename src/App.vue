<template>
  <div id="app">
    <router-view name="header" />
    <div class="wrapper">
      <router-view />
    </div>
    <router-view name="footer" />
  </div>
</template>
<script>
export default {};
</script>
<style>
html {
  scroll-behavior: smooth;
}
/* input:-internal-autofill-selected {
  background-color: blue !important;
} */
</style>
