<template>
  <v-app-bar flat color="#ffffff">
    <router-link to="/"
      ><img src="@/assets/Google_Drive_Logo.png" height="40px" width="40px" class="ml-1"
    /></router-link>
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
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <v-btn fab depressed color="#FFFFFF" small v-on="on">
          <v-icon color="#5F6368">
            mdi-help-circle-outline
          </v-icon>
        </v-btn>
      </template>
      <span>Support</span>
    </v-tooltip>
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <v-btn fab depressed color="#FFFFFF" small v-on="on" class="mr-8">
          <v-icon color="#5F6368">
            mdi-cog-outline
          </v-icon>
        </v-btn>
      </template>
      <span>Settings</span>
    </v-tooltip>
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <v-btn fab depressed color="#FFFFFF" small v-on="on">
          <v-icon color="#5F6368">
            mdi-dots-grid
          </v-icon>
        </v-btn>
      </template>
      <span>Google apps</span>
    </v-tooltip>
    <v-tooltip bottom>
      <template v-slot:activator="{ on }">
        <v-avatar size="32" class="ml-2" v-on="on">
          <img src="@/assets/avatar.png" alt="Profile Picture" />
        </v-avatar>
      </template>
      <span>
        Google Account
      </span>
    </v-tooltip>
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
