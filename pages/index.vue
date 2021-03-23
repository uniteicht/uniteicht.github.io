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
  margin: 0;
  padding: 0;
  padding-left: 10px;
}

h1 {
  color: black;
}
</style>