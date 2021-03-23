<template>
  <div class="outer">
    <h3>
      ACHTUNG: Es handelt sich bei dieser Seite <i>NICHT</i> um den
      <a href="https://uniteich.at" target="_blank">Webauftritt der <i>AktionsGemeinschaft-Linz</i></a>! <br />
      Die haben uns einfach abgekupfert, jegliche Ähnlichkeiten sind also rein
      zufällig. Viel mehr handelt es sich hier um wichtige Vertretungsarbeit!
    </h3>
    <div class="global_wrapper">
      <div class="sidebar">
        <img id="logo" src="/favicon.ico" style="width: 250px" />
        <div class="nav">
          <NuxtLink to="/about">ÜBER UNS</NuxtLink>
        </div>
        <div class="nav">
          <a
            href="https://github.com/uniteicht/uniteicht.github.io"
            target="_blank"
            >MITMACHEN</a
          >
        </div>
        <div class="nav">
          <NuxtLink to="/">ERREICHT!</NuxtLink>
        </div>
        <div class="nav">
          <NuxtLink to="/card">UNITEICHT.CARD</NuxtLink>
        </div>
        <div class="nav">
          <a href="https://anastory.tumblr.com/" target="_blank">BLOG</a>
        </div>
      </div>
      <div class="center">
        <Nuxt />
      </div>
    </div>
  </div>
</template>

<style>
html,
body,
.outer,
#__layout,
#__nuxt {
  height: 100%;
}

.global_wrapper {
  height: 100%;
  background-color: #f26f22;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: white;
}

.sidebar {
  background-color: #ededed;
  width: 20%;
  height: 100%;
  float: left;
  padding: 10px;
}

.center {
  height: 100%;
  float: left;
  width: 80%;
  padding-top: 100px;
  padding-left: 200px;
}

.nav {
  cursor: pointer;
  font-size: 35px;
  text-align: right;
  padding-right: 20px;
  margin: 10px;
  float: right;
}

a {
  color: #f26f22;
  text-decoration: none;
  font-weight: bold;
}

a:hover {
  color: #f26f22;
  text-decoration: none;
  font-weight: bold;
}

#logo {
  float: right;
}
</style>
