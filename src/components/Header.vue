<template>
  <header>
    <span class="headshot"></span>
    <b-nav class="navbar">
      <b-nav-item to="/" exact exact-active-class="active">About</b-nav-item>
      <b-nav-item to="/works" exact exact-active-class="active">Works</b-nav-item>
      <b-nav-item to="/notes" exact exact-active-class="active">Notes</b-nav-item>
      <div>
        <input type="checkbox" id='theme-switch' class='theme-switch sr-only' v-model="darkMode"/>
        <label for='theme-switch'>
          <span v-if="darkMode === true" class="img-switch">
            <img alt="logo" src="@/assets/images/dark.png" width="20">
          </span>
          <span v-else class="img-switch">
            <img alt="logo" src="@/assets/images/light.png" width="20">
          </span>
        </label>
      </div>
    </b-nav>
  </header>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'Header',
  components: {
  },
  data() {
      return {
          darkMode: false,
      }
  },
  mounted() {
      // set page title
      document.title = 'Ugonna T';
      // set 'app-background' class to body tag
      let bodyElement = document.body;
      bodyElement.classList.add("app-background");
      // check for active theme
      let htmlElement = document.documentElement;
      let theme = localStorage.getItem("theme");
      if (theme === 'dark') {
          htmlElement.setAttribute('theme', 'dark')
          this.darkMode = true
      } else {
          htmlElement.setAttribute('theme', 'light');
          this.darkMode = false
      }
  },
  watch: {
      darkMode: function () {
          // add/remove class to/from html tag
          let htmlElement = document.documentElement;
          if (this.darkMode) {
              localStorage.setItem("theme", 'dark');
              htmlElement.setAttribute('theme', 'dark');
          } else {
              localStorage.setItem("theme", 'light');
              htmlElement.setAttribute('theme', 'light');
          }
      }
  }
}
</script>
<style scoped>

</style>