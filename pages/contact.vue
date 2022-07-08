<template>
  <div>
    <div>
      <v-img :src="require(`@/assets/images/3.png`)" height="700">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">
            <strong class="yellow--text text--darken-4"> Contact us </strong>
          </div>
        </v-row>
      </v-img>
</div>    <!-- <div width="100%">
    <img
      :src="require(`/assets/images/3.png`)"  
    />
    </div>
    <v-row class="fill-height" align="center" justify="center">
      <div class="text-h2">
        <strong> CONTACT US </strong>
      </div>
    </v-row> -->
    <!-- </v-img> -->
    <br />
    <v-container>
      <h2 class="text-center">Start Your Journey and Get in Touch</h2>
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
      <p>
         Please feel free to contact us regarding any of our services using the
        following details:
      </p>
    </v-container>
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="6" md="6">
          <div class="map text--primary yellow--text text--darken-3">
            <span>
              <v-icon medium color="blue darken-1"> mdi-map-marker </v-icon>
              <strong> Address:</strong><br />
              Guybrand Limited,<br />
              Office 973,<br />
              58 Peregrine Road,<br />
              Illford IG6 3SZ
            </span>
          </div>
        </v-col>
        <v-col cols="12" sm="6" md="6">
          <div class="map text--primary yellow--text text--darken-3">
            <span>
              <v-icon medium color="blue darken-1"> mdi-phone </v-icon>
              <strong>Landline:</strong>02071830754
              <br />
               <v-icon medium color="blue darken-1"> mdi-email </v-icon>
              <strong>Email:</strong>wohlig@gmail.com
            </span>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <h2 class="yellow--text text--darken-3 text-center">WHERE WE ARE</h2>
      <br />
      <div class="underline1"></div>
      <br />
      <v-row>
        <div>
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d43109.46404148012!2d6.139331415419217!3d47.52221401973193!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47928c21dbead7ab%3A0x409ce34b30f0970!2s70230%20Filain!5e0!3m2!1sen!2sfr!4v1640189073328!5m2!1sen!2sfr"
            width="1150"
            height="600"
            loading="lazy"
          ></iframe>
        </div>
      </v-row> </v-container
    ><br />
    <div class="footer" style="color: grey darken-2">
      <v-row class="foot">
        <span>
          <v-img
            :src="require(`@/assets/images/2.png`)"
            width="65%"
            height="37%"
          ></v-img
          ><br />
          <!-- <v-btn text href="/services"> services </v-btn> -->
          <p style="color: blue">
            About <br />
            Sevices<br />
            Contact
          </p>
        </span>
      </v-row>
    </div>
  </div>
</template>
<script>
export default {
  name: "contact",
};
</script>
<style>
.underline1 {
  height: 2px;
  width: 1140px;
  background-color: rgb(136, 136, 212);
  border-radius: 8px;
  margin-bottom: 16px;
  align-items: inherit;
}
.map {
  display: flex;
  color: grey;
}
.footer {
  background-color: grey;
  color: white;
  padding: 80px;
}

.foot{
justify-content: center;
}
</style>
