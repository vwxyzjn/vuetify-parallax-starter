<template>
  <v-app light>
    <v-toolbar class="white">
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <main>
      <section>
        <v-parallax :src="require('@/assets/background1.jpg')" height="380">
          <v-layout column align-center justify-center>
            <h2 class="teal--text text--lighten-2 mb-2">Parallax Template</h2>
            <div class="white--text headline mb-3">A modern responsive front-end framework based on Material Design</div>
            <v-btn light large class="teal lighten-2 white--text">Get Started</v-btn>
          </v-layout>
        </v-parallax>

        <div id="content">
          <v-layout row wrap class="my-5" >
            <v-flex xs12 sm4>
              <v-card class="elevation-0">
                <v-card-media height="45px" class="text-xs-center">
                  <v-icon x-large class="blue--text">flash_on</v-icon>
                </v-card-media>
                <v-card-title primary-title>
                  <div class="headline text-xs-center" style="width:100%">Speeds up development</div>
                </v-card-title>
                <v-card-text>
                  We did most of the heavy lifting for you to provide
                  a default stylings that incorporate our custom components.
                  Additionally, we refined animations and transitions to 
                  provide a smoother experience for developers.
                </v-card-text>
              </v-card>
            </v-flex>

            <v-flex xs12 sm4>
              <v-card class="elevation-0">
                <v-card-media height="45px" class="text-xs-center">
                  <v-icon x-large class="blue--text">group</v-icon>
                </v-card-media>
                <v-card-title primary-title>
                  <div class="headline text-xs-center" style="width:100%">User Experience Focused</div>
                </v-card-title>
                <v-card-text>
                  By utilizing elements and principles of Material Design, 
                  we were able to create a framework that incorporates components
                  and animations that provide more feedback to users. Additionally,
                  a single underlying responsive system across all platforms allow
                  for a more unified user experience.
                </v-card-text>
              </v-card>
            </v-flex>

            <v-flex xs12 sm4>
              <v-card class="elevation-0">
                <v-card-media height="45px" class="text-xs-center">
                  <v-icon x-large class="blue--text">settings</v-icon>
                </v-card-media>
                <v-card-title primary-title>
                  <div class="headline text-xs-center" style="width:100%">Easy to work with</div>
                </v-card-title>
                <v-card-text>
                  We have provided detailed documentation as well as specific code
                  examples to help new users get started. We are also always open 
                  to feedback and can answer any questions a user may have about 
                  Materialize.
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </div>
      </section>

      <section>
        <v-parallax :src="require('@/assets/background2.jpg')" height="380">
          <v-layout column align-center justify-center>
            <h4 class="white--text">A modern responsive front-end framework based on Material Design</h4>
          </v-layout>
        </v-parallax>
      </section>

      <section>
        <div id="content">
          <v-layout row wrap class="my-5" >
            <v-flex xs12>
              <v-card class="elevation-0">
                <v-card-title primary-title>
                  <div class="headline text-xs-center" style="width:100%">Contact Us</div>
                </v-card-title>
                <v-card-text>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam scelerisque id nunc nec volutpat. 
                  Etiam pellentesque tristique arcu, non consequat magna fermentum ac. Cras ut ultricies eros. 
                  Maecenas eros justo, ullamcorper a sapien id, viverra ultrices eros. Morbi sem neque, posuere 
                  et pretium eget, bibendum sollicitudin lacus. Aliquam eleifend sollicitudin diam, eu mattis nisl 
                  maximus sed. Nulla imperdiet semper molestie. Morbi massa odio, condimentum sed ipsum ac, gravida 
                  ultrices erat. Nullam eget dignissim mauris, non tristique erat. Vestibulum ante ipsum primis in 
                  faucibus orci luctus et ultrices posuere cubilia Curae;
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </div>
      </section>

      <section>
        <v-parallax :src="require('@/assets/background3.jpg')" height="380">
          <v-layout column align-center justify-center>
            <h4 class="white--text">A modern responsive front-end framework based on Material Design</h4>
          </v-layout>
        </v-parallax>
      </section>


      <div id="footer" class="teal darken-1">
        <v-layout row wrap style="width:70%;margin:auto" class="my-5">
          <v-flex xs12 sm6>
            <div class="headline white--text">Company Bio</div>
            <div class="white--text mt-3">
              We are a team of college students working on this project like 
              it's our full time job. Any amount would help support and continue 
              development on this project and is greatly appreciated.
            </div>
          </v-flex>
          <v-flex xs12 sm3>
            <div class="headline white--text">Settings</div>
            <div class="white--text mt-3">
              <a>Link1</a> <br>
              <a>Link2</a> <br>
              <a>Link3</a> <br>
              <a>Link4</a> <br>
            </div>
          </v-flex>
          <v-flex xs12 sm3>
            <div class="headline white--text">Connect</div>
            <div class="white--text mt-3">
              <a>Link1</a> <br>
              <a>Link2</a> <br>
              <a>Link3</a> <br>
              <a>Link4</a> <br>
            </div>
          </v-flex>
        </v-layout>
      </div>
      <footer class="teal darken-2">
        <v-layout row wrap style="width:70%;margin:auto" class="my-2">
          <v-flex xs12>
            <div class="white--text">
              Made by Costa Huang
            </div>
          </v-flex>
        </v-layout>
      </footer>
    </main>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        title: 'Your Logo'
      }
    }
  }
</script>

<style lang="stylus">
  @import './stylus/main'
</style>

<style>
.toolbar__title {
  margin-left: 15%;
}

#subtitle {
  font-weight: 200!important;
}

#content {
  width: 70%;
  margin: auto;
}

#footer {
  overflow: auto;
}
.card {
  background-color: #fafafa!important;
}
footer {
  overflow: auto;
}
a {
  color: #fff;
}
</style>