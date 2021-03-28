<template>
  <div class="outer">
    <h3>
      ACHTUNG: Es handelt sich bei dieser Seite <i>NICHT</i> um den
      <a href="https://uniteich.at" target="_blank"
      >Webauftritt der <i>AktionsGemeinschaft-Linz</i> <i class="fas fa-external-link-alt"></i></a
      >! <br/>
      Die haben uns einfach abgekupfert, jegliche Ähnlichkeiten sind also rein
      zufällig. Viel mehr handelt es sich hier um wichtige
      Vertretungsarbeit!!1einself
    </h3>
    <div class="global_wrapper">
      <div class="sidebar">
        <NuxtLink to="/"><img id="logo" src="/favicon.ico" style="width: 250px"/></NuxtLink>
        <div class="nav">
          <NuxtLink to="/about">ÜBER UNS</NuxtLink>
        </div>
        <div class="nav">
          <a
            href="https://github.com/uniteicht/uniteicht.github.io"
            target="_blank"
          >MITMACHEN <i class="fas fa-external-link-alt"></i></a
          >
        </div>
        <div class="nav">
          <NuxtLink to="/">ERREICHT!</NuxtLink>
        </div>
        <div class="nav">
          <NuxtLink to="/card">UNITEICHT.CARD</NuxtLink>
        </div>
        <div class="nav">
          <a href="https://anastory.tumblr.com/" target="_blank">BLOG <i class="fas fa-external-link-alt"></i></a>
        </div>

        <div class="imprint">
          <div class="wr-social">
            <a href="https://onlyfans.com/u128981358" target="_blank"><img
              src="/img/OnlyFans_Social_Icon_Rounded_Blue.svg" class="social onlyfans-logo" /></a>
            <a href="https://anastory.tumblr.com/" target="_blank"><i
               class="fab fa-tumblr social"></i></a>
            <a href="https://www.instagram.com/tag.jku.uniteicht/" target="_blank"><i
              class="fab fa-instagram social"></i></a>
             
              
          </div>
          <NuxtLink to="/imprint">Credits</NuxtLink>
          <NuxtLink to="/imprint">Impressum</NuxtLink>
        </div>
      </div>
      <div class="center">
        <Nuxt/>
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
  font-weight: 400;
  font-size: 4em;
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


.wr-social {
  float: right;
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
  min-width: 360px;
  height: auto;
  float: left;
  padding: 10px;
}

.center {
  padding-top: 100px;
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
  display: block;
  margin-left: auto;
  margin-right: auto;
}


@media only screen and (min-width: 768px) {
  .wr-social {
    float: right;
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
    min-width: 360px;
    float: left;
    padding: 10px;
  }

  .center {
    height: auto;
    float: left;
    width: 70%;
    padding-top: 100px;
    padding-left: 200px;
  }

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



  #logo {
    float: right;
  }
}




</style>
