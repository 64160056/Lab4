<template>
  <v-app :theme="theme">
    <v-app-bar>
      <v-spacer></v-spacer>

      <v-btn
        :prepend-icon="theme === 'light' ? mdiWeatherSunny : mdiWeatherNight"
        @click="onClick"
        >Toggle Theme</v-btn
      >
    </v-app-bar>
    <v-navigation-drawer expand-on-hover rail permanent>
      <v-list>
        <v-list-item
          prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
          title="Sandra Adams"
          subtitle="sandra_a88@gmailcom"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item
          :prepend-icon="mdiFolder"
          title="My Files"
          value="myfiles"
          to="/my-files-view"
        ></v-list-item>
        <v-list-item
          :prepend-icon="mdiAccountMultiple"
          title="My Profile"
          value="shared"
          to="/shared-with-me"
        ></v-list-item>
        <v-list-item
          :prepend-icon="mdiStar"
          title="Starred"
          value="starred"
          to="/starred-viwe"
        ></v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import { ref } from "vue";
import {
  mdiFolder,
  mdiAccountMultiple,
  mdiStar,
  mdiWeatherSunny,
  mdiWeatherNight,
  mdiCursorPointer,
  mdiVuetify,
  mdiCheckboxMarkedCircle,
} from "@mdi/js";
const theme = ref("light");

function onClick() {
  theme.value = theme.value === "light" ? "dark" : "light";
}
</script>
