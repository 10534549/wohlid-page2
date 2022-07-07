<template>
  <v-app>
    <v-app-bar :clipped-left="clipped" fixed shrink-on-scroll prominent  elevation="0" 
    
    class="text-xs-center">
<v-toolbar-side-icon>
        <v-img
          :src="require(`@/assets/images/2.png`)"
          width="100%"
          height="100%"
        ></v-img>
        
      </v-toolbar-side-icon>
            <v-spacer />
      <v-btn text href="/"> Home </v-btn>
       <!-- <NuxtLink to="/home">Home</NuxtLink>

       <NuxtLink to="/about">About</NuxtLink> -->
       <v-btn text  href="/about"> About </v-btn>
      <v-btn text  href="/services"> Services </v-btn>
      
     
      <v-btn text  href="/contact"> Contact </v-btn>
      
      
    </v-app-bar>

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        
      ],
      
      title: "Vuetify.js",
    };
  },
};
</script>
<style scoped>
.first{
justify-content: center;
}
.nav .btn{
  text-align:center
}
</style>