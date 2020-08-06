<template>
  <header id="top-header">
    <Container>
      <b-container>
        <b-row align-v="center">
          <b-col col="4">
            <span class="headshot"></span>
          </b-col>
          <b-col col="7" id="list-div">
            <b-nav>
              <b-nav-item to="/" exact exact-active-class="active">Home</b-nav-item>
              <b-nav-item to="/about" exact exact-active-class="active">About</b-nav-item>
              <b-nav-item to="/about" exact exact-active-class="active">Notes</b-nav-item>
              <div class="">
                <input type="checkbox" id='theme-switch' class='theme-switch sr-only' v-model="darkMode"/>
                <label for='theme-switch'>
                  <span v-if="darkMode === true">
                    <img alt="logo" src="@/assets/images/light.png" width="20">
                  </span>
                  <span v-else>
                    <img alt="logo" src="@/assets/images/dark.png" width="20">
                  </span>
                </label>
              </div>
            </b-nav>
          </b-col>
        </b-row>
      </b-container>
    </Container>
  </header>
</template>

<script>
// @ is an alias to /src
import Container from '@/components/Container.vue'
export default {
  name: 'Header',
  components: {
    Container
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