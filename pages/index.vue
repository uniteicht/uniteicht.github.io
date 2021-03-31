<template>
  <div class="wrapper">
    <h1>FÜR DICH ERREICHT</h1>
    <MemeList />
  </div>
</template>

<style>
</style>

<script>
export default {
  middleware({ redirect }) {
    const ls = window.localStorage;
    if (!ls.getItem("first")) {
      ls.setItem("first", false);
      return redirect("/about");
    }
  },
};
</script>

<style>
.wrapper {
  width: 100%;
  height: 100%;
  margin: auto;
}

h1 {
  color: black;
  padding: 1em;
}
</style>
