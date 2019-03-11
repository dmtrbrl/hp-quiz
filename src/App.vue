<template>
  <div class="app">
    <header class="app-header">
      <span class="app-header-text">
        Show on
        <a href="https://github.com/dmtrbrl/hp-quiz">Github</a>
      </span>
      <h1 class="app-heading">
        <svg
          width="60"
          height="60"
          viewBox="0 0 60 60"
          xmlns="http://www.w3.org/2000/svg"
          class="app-heading-icon"
        >
          <path
            d="M28.745 57.76a3.116 3.116 0 1 0 5.68-2.565L24.203 32.559l16.332 2.085a3.065 3.065 0 0 0 2.895-1.229 3.117 3.117 0 0 0 .347-3.126L31.315 2.252a3.115 3.115 0 0 0-5.692 2.531l10.213 22.98-16.37-2.09a3.085 3.085 0 0 0-2.901 1.236 3.117 3.117 0 0 0-.335 3.136L28.745 57.76z"
          ></path>
        </svg>
        <span>Harry Potter</span>
        <span>Movies Quiz</span>
      </h1>
      <span class="app-header-text">
        Thanks
        <a href="https://giphy.com/" target="_blank">GIPHY</a> for the gifs
      </span>
    </header>
    <Quiz url="https://api.myjson.com/bins/19efxu"/>
  </div>
</template>

<script>
import Quiz from "./components/Quiz.vue";

export default {
  name: "app",
  components: {
    Quiz
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Merriweather:400,700");
@import url("https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css");

* {
  box-sizing: border-box;
}

html {
  height: 100%;
}

body {
  height: 100%;
  background: #020815;
  color: #eee;
}

.app {
  min-height: 100%;
  padding: 95px 15px 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Merriweather", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
.app-header {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 95px;
  padding: 15px;
  display: flex;
  justify-content: space-between;
  font-size: 11px;
}
.app-header a {
  color: #eee;
  text-decoration: none;
  border-bottom: 1px solid rgba(238, 238, 238, 0.5);
}
.app-heading {
  position: absolute;
  top: 50px;
  left: 50%;
  margin: 0;
  padding-left: 20px;
  font-size: 14px;
  line-height: 15px;
  transform: translateX(-50%);
  cursor: default;
  user-select: none;
}
@media (min-width: 600px) {
  .app-header {
    height: 90px;
    padding: 30px 15px;
    align-items: center;
  }
  .app-heading {
    top: 30px;
  }
}
.app-heading-icon {
  position: absolute;
  top: 1px;
  left: -5px;
  fill: #eee;
  width: 26px;
  height: 26px;
}
.app-heading span {
  display: block;
}
.app-header-text {
  opacity: 0.5;
}
</style>
