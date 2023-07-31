<script setup lang="ts">
import ProductPreview from '~/components/ProductPreview.vue'
</script>

<template>
  <v-app>
    <v-main>
      <v-container
        class="fill-height d-flex flex-column"
      >
        <v-spacer />
        <div>
          <ProductPreview />
        </div>
        <v-spacer />
        <div class="attribution text-center w-100">
          Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
          Coded by <a href="https://github.com/Antoine340">@Antoine340</a>.
        </div>
      </v-container>
    </v-main>
  </v-app>
</template>
