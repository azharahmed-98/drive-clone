<template>
  <v-app-bar flat color="#ffffff">
      <img src="@/assets/Google_Drive_Logo.png" height="40px" width="40px" class="ml-1" />
      <a href="/" class="ml-2 mr-16 font-weight-regular text-h5">Drive</a>
    <v-text-field
      color="#5F6368"
      placeholder="Search in Drive"
      solo
      flat
      single-line
      background-color="#F1F3F4"
      prepend-inner-icon="mdi-magnify"
      append-icon="mdi-tune"
      class="mt-7 ml-16 rounded-lg"
    >
    </v-text-field>
    <v-spacer></v-spacer>
  </v-app-bar>
</template>

<script>
export default {
  name: 'Navbar',
  methods: {},
};
</script>

<style scoped>
a {
  color: #5f6368 !important;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}
</style>
