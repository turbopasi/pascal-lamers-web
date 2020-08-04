<template>
  <div class="layout">
    <header class="header">
      <nav class="navigation">
        <!-- Nav Bar Content -->
        <div class="logo">
          <g-image src="~/assets/lamers_text_only.svg" />
        </div>
        
        <div class="menu">
          <p>Intro</p>
          <p>Pricing</p>
        </div>
        
        <div class="cta">
          <button>Auftrag erstellen</button>
        </div>

      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>

* {
  margin : 0;
  padding : 0;
  font-weight: 500;
}

body {
  font-family: 'Rubik';
  /* margin:0;
  padding:0;
  line-height: 1.5;
  background : pink; */
}

.layout {
  /* max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
  background : pink; */
}

header.header {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 9999;
  width: 100%;
  height: 80px;
  background-color: none;
}

nav.navigation {
  height : 100%;
  display : flex;
  align-items: center;
  width: 80%;
  margin:0 auto;
}

nav.navigation .logo {
  flex : 1;
}

nav.navigation .menu {
  display:inline-flex
}

nav.navigation .menu p{
  margin : 0px 10px;
}

nav.navigation .cta {
  flex: 1;
}

</style>
