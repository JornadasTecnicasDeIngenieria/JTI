<template>
  <div>
    <Header />
    <Nuxt class="bg-jti-gray" />
    <Footer />
  </div>
</template>

<style>
@import "https://cdnjs.cloudflare.com/ajax/libs/material-design-icons/3.0.1/iconfont/material-icons.min.css";
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400;1,600;1,700&display=swap');

html {
  font-family: "Raleway", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

.wrapper {
  max-width: 1200px;
  margin: 0 auto;
}

h1 {
  font-size: 3em;
  font-family: "Montserrat";
  font-weight: bold;
  color: white;
}

h2 {
  font-size: 2em;
  font-family: "Montserrat";
  font-weight: bold;
  color: #5c068c;
}

@media (max-width: 800px) {
  h2 {
    text-align: center;
  }
}

h3 {
  font-size: 2em;
  font-family: "Montserrat";
  color:white;
}

h4 {
  font-size: 1em;
  font-family: "Montserrat";
  font-weight: bold;
  color: #5c068c;
}

</style>
