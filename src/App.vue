<template>
  <div id="app">
    <Header />
    <router-view/>
    <section class="hire-me">
      <article>
        <h2>I can help.</h2>			
        <h3>I’m currently available for freelance work.</h3>		
        <div class="help-text">
          <p>If you have a project that you want to get started, think you need my help with something or just fancy saying hey, then get in touch.</p>
        </div>
          <a href="mailto:ugonnathelma@gmail.com" class="mail-button">MESSAGE ME</a>
      </article>
    </section>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
