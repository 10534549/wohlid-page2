<template>
  <div>
    <br/>
    <div>
    <v-card elevation="0">
      <v-carousel
        class="fill-height"
        :continuous="false"
        :cycle="cycle"
        :show-arrows="false"
        hide-delimiter-background
        delimiter-icon="mdi-minus"
        height="678"
      >
        <v-carousel-item
          v-for="(item, i) in items"
          :key="i"
          :src="item.src"
          reverse-transition="fade-transition"
          transition="fade-transition"
        >
          <v-row class="fill-height" align="center" justify="center">
            <div class="text-h2">
              <strong class=" yellow--text text--darken-4"> {{ slide }} Welcome to guy brand limited </strong>
            </div>
          </v-row>
        </v-carousel-item>
      </v-carousel>
    </v-card>
    </div>
    <v-container>
      <h2 class="text-center yellow--text text--darken-4">GUY BRAND LIMITED</h2>
      <br />
      <div class="underline1"></div>
      <br />
      <p>
        Guybrand Limited is a family-run building company. Every home is unique
        and should be perfectly built and designed to meet your needs. The
        Guybrand Limited team is made up of talented and experienced building
        professionals who will discuss all the options available and work with
        you to develop the best solution for your home.
      </p>
    </v-container>
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="6" md="8">
          <v-row class="trail" height="100%">
            <p class="text--primary">
              When it comes to any building project, there is a wealth of
              information available and the options can be overwhelming. Whether
              you’re starting the process of working your way up the property
              ladder, remodelling your living space, or building a dream home,
              it can be tricky to know where to start. We are here to support
              you on every step of the journey.
            </p>
          </v-row>
        </v-col>
        <v-col cols="12" sm="6" md="4">
          <v-img
            :src="require(`@/assets/images/3.png`)"
            width="100%"
            height="100%"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="6" md="4">
          <v-img
            :src="require(`@/assets/images/3.png`)"
            width="100%"
            height="100%"
          ></v-img>
        </v-col>
        <v-col cols="12" sm="6" md="8">
          <v-row class="trail" height="100%">
            <p class="text--primary">
              When it comes to any building project, there is a wealth of
              information available and the options can be overwhelming. Whether
              you’re starting the process of working your way up the property
              ladder, remodelling your living space, or building a dream home,
              it can be tricky to know where to start. We are here to support
              you on every step of the journey.
            </p>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="6" md="6">
          <h2 class="blue--text text--darken-4 text-center">Read to go?</h2>
          <br />
          <v-row>
            <p>
              If you have architectural plans and are looking for professional
              builders, find out more about the Guybrand Limited Bespoke Build
              service.
            </p>
          </v-row>
        </v-col>
        <v-col cols="12" sm="6" md="6">
          <h2 class="blue--text text--darken-4 text-center">
            Just Starting Out?
          </h2>
          <br />
          <v-row>
            <p>
              If you’re at the beginning of your journey and need someone to
              take care of everything, find out more about the Guybrand Limited
              Design, Planning & Build service.
            </p>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <div class="footer" style="color: grey darken-2">
      <v-row>
        <v-col style="color: grey" cols="12" sm="5" md="4">
          <v-img
            :src="require(`@/assets/images/2.png`)"
            width="37%"
            height="25%"
          ></v-img
          ><br />
          <!-- <v-btn text href="/services"> services </v-btn> -->
          <p style="color: blue">
            About <br />
            Sevices<br />
            Contact
          </p>
        </v-col>
        <v-col cols="12" sm="6" md="4">
          <h2 style="color: blue">Get in touch</h2>
          <div class="underline2"></div>
          <p class="blue--text text--darken-4">
            Please feel free to get in touch with us regarding any of our
            services using the following details
          </p>
          <ul style="color: black">
            <li v-for="fruit in fruits">{{ fruit }}</li>
          </ul>
        </v-col>
        
        <v-col cols="12" sm="6" md="4">
          <h2 style="color: blue">Where we are</h2>
          <div class="underline2"></div>
          <div>
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d43109.46404148012!2d6.139331415419217!3d47.52221401973193!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47928c21dbead7ab%3A0x409ce34b30f0970!2s70230%20Filain!5e0!3m2!1sen!2sfr!4v1640189073328!5m2!1sen!2sfr"
              width="350"
              height="220"
              loading="lazy"
            ></iframe>
          </div>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      items: [
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],

      slides: ["First", "Second", "Third", "Fourth", "Fifth"],
      fruits: [
        "Office 973,58 Peregrine Road,Ilford IG6 3SZ",
        "Phone: 0207 183 0754",
        "Email: sales@guybrand.co.uk",
      ],
    };
  },
};
</script>
<style scoped>
.underline1 {
  height: 2px;
  width: 1140px;
  background-color: rgb(136, 136, 212);
  border-radius: 8px;
  margin-bottom: 16px;
  align-items: inherit;
}
.footer {
  background-color: grey;
  color: white;
  padding: 80px;
}
.underline2 {
  height: 2px;
  width: 250px;
  background-color: rgb(136, 136, 212);
  border-radius: 8px;
  margin-bottom: 16px;
  align-items: inherit;
}
</style>
