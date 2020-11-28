<template>
  <main>
    <section class="short-intro">
      <article>
        <span class="headshot2"></span>
        <h3>Hi.</h3>
        <div class="short-text">
          <p>
            I'm a web designer / developer based in Berlin, Germany. I have a
            passion for web design and love to create for web and mobile
            devices.
          </p>
        </div>
      </article>
    </section>
    <section class="skills">
      <h2>What can I do.</h2>
      <b-container class="skills-container">
        <b-row>
          <b-col cols="4" class="short-image first-image">
            <span class="headshot2"></span>
          </b-col>
          <b-col cols="6" class="deets design">
            <h3>Design what you want.</h3>
            <p>I like to keep it simple. My goals are to focus on typography, content and conveying the message that you want to send.</p>
          </b-col>
        </b-row>
        <b-row>
          <b-col cols="6" class="deets develop">
            <h3>Develop what you need.</h3>
            <p>I'm a developer, so I know how to create your website to run across devices using the latest technologies available.</p>
          </b-col>
          <b-col cols="4" class="short-image second-image">
            <span class="headshot2"></span>
          </b-col>
        </b-row>
      </b-container>
    </section>
  </main>
</template>

<script>
export default {
  name: "Skills",
  components: {},
};
</script>
