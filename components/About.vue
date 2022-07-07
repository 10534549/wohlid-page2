<template>
  <v-card class="blue darken-2" max-width="320" elevation="1">
    <!-- <pre>{{ card }}</pre> -->
    <div>
      <v-card-title class="yellow--text">
        {{ card.title }}
      </v-card-title>
      <div class="underline2"></div>

      <v-card-subtitle>
        {{ card.paragraph }}
      </v-card-subtitle>
    </div>
  </v-card>
</template>
<script>
export default {
  props: {
    card: {
      type: Object,
      default: () => {},
    },
  },
  data: () => ({
    show: false,
    reveal: false,
  }),
  watch: {
    title: function (newVal) {
      console.log(newVal);
    },
  },
};
</script>
<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}

.underline2 {
  height: 1px;
  width: 320px;
  background-color: blue;
  border-radius: 8px;
  margin-bottom: 16px;
  align-items: inherit;
}
</style>
