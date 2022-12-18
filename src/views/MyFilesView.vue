<script setup lang="ts">
import FancyButton from "@/components/FancyButton.vue";
import { mdiCardsHeartOutline } from "@mdi/js";
import { mdiCursorDefaultClickOutline } from "@mdi/js";
</script>

<template>
  <v-container>
    <v-row>
      <v-col
        ><FancyButton
          ><v-icon :icon="mdiCardsHeartOutline"></v-icon>Love Me
          <template v-slot:tall> Tall </template>
        </FancyButton></v-col
      >
      <v-col
        ><FancyButton
          >Click Me
          <template #tall>
            <v-icon :icon="mdiCursorDefaultClickOutline"
          /></template>
        </FancyButton>
      </v-col>
    </v-row>
  </v-container>
</template>
