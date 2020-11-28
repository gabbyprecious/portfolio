<template>
  <main class="portfolio">
    <section class="details">
      <div class="work">
        <h1>Work</h1>
      </div>
    </section>
    <section class="work-div work-green">
      <div class="img-div">
        <img
          alt="land"
          src="@/assets/images/work1.jpg"
          width="900"
          height="441"
          style="display: inline;"
        />
      </div>
      <div class="work-details">
        <h2>Table Reservation</h2>
        <h3>Interface Design / UI</h3>
        <p>
          As an exploration in product design and architecture I have been
          working on an idea for a restaurant reservation system. Thoroughly
          challenging thinking through the product design but ultimately
          rewarding.
        </p>
        <button type="submit">Check it Out</button>
      </div>
    </section>
    <section class="work-div work-red">
      <div class="img-div">
        <img
          alt="land"
          src="@/assets/images/work1.jpg"
          width="900"
          height="441"
          style="display: inline;"
        />
      </div>
      <div class="work-details">
        <h2>Netlify</h2>
        <h3>Built Site</h3>
        <p>Built a Dynamic site with information given by a designer</p>
        <button type="submit">Check it Out</button>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "Work",
  components: {},
};
</script>

<style></style>
