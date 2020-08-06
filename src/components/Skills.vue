<template>
  <main>
    <Container>
      <section>
        <b-container>
          <b-row>
            <b-col col="12">
              <article>
                <figure>
                  <span class="headshot2"></span>
                </figure>
                <h3>Hi.</h3>
                <p>I'm a web designer / developer based in Berlin, Germany. I have a passion for web design and love to create for web and mobile devices.</p>
              </article>
            </b-col>
          </b-row>
        </b-container>
      </section>
      <section>
        <b-container>
          <b-row>
            <b-col col="12">
              <article>
                <header>
                  <h2>What can I do</h2>
                </header>
                <b-row>
                  <b-col col="4">
                    <figure>
                      <span class="headshot2"></span>
                    </figure>
                  </b-col>
                  <b-col col="8">
                    <div class="deets">
                      <h3 style="font-size: 2em;">Design what you want.</h3>
                      <p>I like to keep it simple. My goals are to focus on typography, content and conveying the message that you want to send.</p>
                    </div>
                    <div id="develop" class="row">
                      <div class="col-md-4 col-md-push-7">
                        <div class="home-dev-info">
                          <figure>
                            <span class="headshot2"></span>
                          </figure>
                          <div class="bubble left">
                            <div class="bubbling-dev-icons-vert"></div>
                          </div>			
                        </div>
                      </div> <!-- col -->
                      <div class="col-md-6 col-md-pull-3">
                        <div class="deets">
                          <h3>Develop what you need.</h3>
                          <p>I'm a developer, so I know how to create your website to run across devices using the latest technologies available.</p>
                        </div>            
                      </div> <!-- col -->
                    </div>
                  </b-col>
                </b-row>
              </article>
            </b-col>
          </b-row>
        </b-container>
      </section>
      <section id="i-can-help">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <article>
                <header class="">
                  <h2>I can help.</h2>			
                  <h3>I’m currently available for freelance work.</h3>		
                </header>
                <p>If you have a project that you want to get started, think you need my help with something or just fancy saying hey, then get in touch.</p>
                <p class="btn-hldr">
                  <a href="mailto:sean.e.halpin@gmail.com" class="main-btn email-lnk">message me <i class="email"></i></a>
                </p>
              </article>
            </div>
          </div>
        </div>
      </section>
    </Container>
  </main>
</template>

<script>
import Container from '@/components/Container.vue'

export default {
  name: 'Skills',
  components: {
    Container
  }
}
</script>