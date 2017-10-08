<template>
  <div id="app">
    <header>
      <h1>
        Maxence<br>
        Aici
      </h1>
      <p>maker - software engineering, design, video</p>
    </header>
    <main>
      <a href="/files/Maxence_Aici_CV.pdf">cv</a>
      <a href="https://github.com/mininao">github</a>
      <a href="mailto:maxence@aici.me">email</a>
    </main>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
@font-face {
  font-family: 'g-web';
  src:  url('../static/fonts/g-Black.woff') format('woff');
  font-weight: 800;
}
$color-dark: #1B1B1B;
$color-accent-green: #00EBAF;
$color-accent-blue: #3FDBF8;
$color-accent-purple: #92B6F9;
$color-accent-red: #FF7D9E;

body {
  margin: 0;
  background-color: $color-dark;
  font-family: 'g-web', Helvetica, Arial, sans-serif;
  font-weight: 800;
}
#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
header {
      margin: 2rem;
  h1 {
    text-transform: uppercase;
    color: $color-accent-blue;
    font-size: 2rem;
    margin: 0;
  }
  p {
    color: white;
    opacity: 0.8;
    font-size: 1rem;
  }
}
main {
  position:absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  flex-grow: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  a {
    margin: 0 1rem;
    font-size: 1.5rem;
    text-decoration: none;
    color: $color-accent-green;
    &:nth-child(2) {
      color: $color-accent-red;
    }
    &:nth-child(3) {
      color: $color-accent-purple;
    }
  }
}
</style>
