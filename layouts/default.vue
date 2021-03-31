<template>
  <div class="outer">
    <script>
      function qak() {
        new Audio("qak.mp3").play();
        setTimeout(() => {
          document.getElementById("logo").src = "favicon2.png";
          setTimeout(() => {
            document.getElementById("logo").src = "favicon.ico";
          }, 400);
        }, 200);
      }
    </script>
    <span font-size="0.3em">
      ACHTUNG: Es handelt sich bei dieser Seite <i>NICHT</i> um den
      <a href="https://uniteich.at" target="_blank"
        >Webauftritt der <i>AktionsGemeinschaft-Linz</i>
        <i class="fas fa-external-link-alt"></i></a
      >!<br />
      Die haben uns einfach abgekupfert, jegliche Ähnlichkeiten sind also rein
      zufällig. Viel mehr handelt es sich hier um wichtige
      Vertretungsarbeit!!1einself
    </span>
    <div class="global_wrapper" onclick="qak()">
      <div class="sidebar">
        <a onClick="qak()"><img id="logo" src="/favicon.ico" /></a>
        <div class="nav">
          <NuxtLink to="/about">ÜBER UNS</NuxtLink>
        </div>
        <div class="nav">
          <NuxtLink to="/#content"
            ><span
              onmouseover="this.innerHTML='ERTEICH<b>T</b>'"
              onmouseout="this.innerHTML='ERREICHT'"
            >
              ERREICHT</span
            >!</NuxtLink
          >
        </div>
        <div class="nav">
          <NuxtLink to="/card#content">UNITEICHT.CARD</NuxtLink>
        </div>
        <div class="nav">
          <NuxtLink to="/poesie#content">POESIE-ALBUM</NuxtLink>
        </div>
        <div class="nav">
          <NuxtLink to="/imprint#content">Impressum</NuxtLink>
        </div>

        <div class="imprint">
          <div class="wr-social">
            <div>
              <a
                href="https://onlyfans.com/u128981358"
                target="_blank"
                title="Onlyfans"
                ><img
                  class="social onlyfans-logo"
                  src="/img/OnlyFans_Social_Icon_Rounded_Blue.svg"
              /></a>
            </div>

            <div>
              <a
                href="https://anastory.tumblr.com/"
                target="_blank"
                title="Tumblr"
                ><i class="fab fa-tumblr social"></i
              ></a>
            </div>

            <div class="even-bigger">
              <a
                href="https://github.com/uniteicht/uniteicht.github.io"
                target="_blank"
                title="Github"
                ><i class="fab fa-github-square"></i
              ></a>
            </div>

            <div class="bigger">
              <a
                href="https://www.instagram.com/tag.jku.uniteicht/"
                target="_blank"
                title="Insta"
                ><i class="fab fa-instagram social"></i
              ></a>
            </div>
          </div>
        </div>
      </div>
      <div class="center" id="content">
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

.social {
  font-size: 1.5em;
}

.onlyfans-logo {
  width: 1em;
  height: 1em;
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

.nav {
  cursor: pointer;
  font-size: 35px;
  text-align: left;
  margin: 10px;
  clear: both;
}

.imprint {
  display: block;
}

.imprint a {
  display: block;
  float: left;
  margin: 5px;
}

#logo {
  width: 100%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}

.wr-social {
  display: flex;
  justify-content: space-between;
}

.imprint {
  display: block;
  padding-right: 20px;
}

.imprint a {
  display: block;
}

.icon {
  height: 1rem;
  margin-top: -8px;
  margin-right: 5px;
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
  float: left;
  padding: 10px;
}

.center {
  height: auto;
  float: left;
  width: 80%;
}

.bigger {
  font-size: 1.2em;
  margin-top: -0.1em;
}

.even-bigger {
  font-size: 1.7em;
  margin-top: -0.26em;
  margin-left: 0.1em;
}

.imprint,
.nav {
  cursor: pointer;
  font-size: 35px;
  text-align: right;
  padding-right: 20px;
  margin: 10px;
  clear: both;
  display: block;
}

.nav a {
  width: 100%;
  text-align: right;
}

@media screen and (max-width: 1200px) {
  .imprint,
  .nav {
    font-size: 25px;
  }
}

@media screen and (max-width: 800px) {
  .imprint,
  .nav {
    font-size: 18px;
  }
}

@media screen and (max-width: 600px) {
  .sidebar {
    width: 100%;
  }
  .nav {
    font-size: 35px;
  }
  .center {
    width: 95%;
    margin-left: 2.5%;
  }
}
</style>
