<template>
  <div>
    <v-container>
      <v-img :src="require(`@/assets/images/3.png`)" height="700">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">
            <strong class=" yellow--text text--darken-4"> About us </strong>
          </div>
        </v-row>
      </v-img>
    </v-container>
    <v-container>
      <div>
        <h2 class="blue--text text--darken-4 text-center">
          Why Choose Guybrand Limited?
        </h2>
      </div>
      <br />
      <v-row>
        <p>
          Guybrand Limited is a family-run company that has grown organically
          into a large professional team of skilled tradesmen. We maintain the
          highest quality of work by only using our own team and partnering with
          leading architectural, surveyor, design and engineering companies.
        </p> </v-row
      ><br />
      <v-row>
        <p>
          Guybrand Limited is a family-run company that has grown organically
          into a large professional team of skilled tradesmen. We maintain the
          highest quality of work by only using our own team and partnering with
          leading architectural, surveyor, design and engineering
          companies.Guybrand Limited is a family-run company that has grown
          organically into a large professional team of skilled tradesmen. We
          maintain the highest quality of work by only using our own team and
          partnering with leading architectural, surveyor, design and
          engineering companies.
        </p>
      </v-row>
    </v-container>

    <v-container>
      <div class="text-center"></div>
      <br />
      <v-row>
        <v-col
          v-for="(item, index) in Abouts"
          :key="index"
          cols="12"
          md="4"
          sm="6"
        >
          <About :card="item" />
        </v-col>
      </v-row>
    </v-container>

    <!-- <template>
      <v-card class="mx-auto" max-width="300">
        <v-card-text>
          <h3>Quality</h3>
          <p class="text--secondary">
            Guybrand Limited is a family-run company that has grown organically
            into a large professional team of skilled tradesmen. We maintain the
            highest quality
          </p>
        </v-card-text>
      </v-card>
    </template> -->
    <br />
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
    <v-container class="footer" style="color: grey darken-2">
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
    </v-container>
  </div>
</template>
<script>
import About from "../components/About.vue";
export default {
  components: { About },
  name: "about",

  data: () => ({
    Abouts: [
      {
        title: "QUALITY",
        paragraph:
          "Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.",
      },
      {
        title: "COST",
        paragraph:
          "Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.",
      },
      {
        title: "TIME",
        paragraph:
          "Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.Guybrand Limited is fully insured for all our work. We provide defects and structural guarantee on all new installations.",
      },
    ],
    fruits: [
      "Office 973,58 Peregrine Road,Ilford IG6 3SZ",
      "Phone: 0207 183 0754",
      "Email: sales@guybrand.co.uk",
    ],
  }),
};
</script>
<style scoped>
.footer {
  background-color: grey;
  color: white;
  padding: 80px;
}
</style>
