<script setup lang="ts">

</script>

<template>
  <v-row
    no-gutters
    class="container"
  >
    <v-col cols="12" md="6">
      <v-img
        :src="$vuetify.display.smAndDown ? 'images/image-product-mobile.jpg' : 'images/image-product-desktop.jpg'"
        class="card-left"
        alt="product"
        width="100%"
        height="100%"
      />
    </v-col>
    <v-col cols="12" md="6">
      <v-card
        elevation="0"
        class="card-right fill-height d-flex flex-column"
        :class="{
          'pa-12': $vuetify.display.smAndUp,
          'pa-6': $vuetify.display.xs,
        }"
      >
        <v-card-subtitle class="product-subtitle mb-4 pa-0">
          PERFUME
        </v-card-subtitle>
        <v-card-title class="pa-0">
          <h1 class="product-title mb-8">
            Gabrielle <br> Essence Eau <br> De Parfum
          </h1>
        </v-card-title>
        <div class="d-flex flex-column">
          <p
            class="opacity-6 product-description"
          >
            A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator for the House of CHANEL.
          </p>
        </div>
        <v-spacer />
        <div
          class="d-inline-flex align-center my-4"
        >
          <h1
            class="price price--color mr-8"
          >
            $149.99
          </h1>
          <h4
            class="price price--small text-decoration-line-through opacity-6"
          >
            $169.99
          </h4>
        </div>
        <v-spacer />
        <v-card-actions class="pa-0">
          <v-btn
            block
            class="add-to-cart-btn text-none text-white"
            variant="flat"
            color="hsl(158, 36%, 37%)"
            size="64"
            rounded="lg"
          >
            <v-img
              src="/images/icon-cart.svg"
              width="24"
              height="24"
              class="mr-4"
            >
            </v-img>
            <h3><b>Add to Cart</b></h3>
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<style scoped lang="scss">
p {
  font-family: 'Montserrat', sans-serif!important;
}
h1 {
  font-family: 'Fraunces', serif!important;
}
.add-to-cart-btn {
  &:hover {
    background-color: #1E4135!important;
  }
}
.card {
  &-left {
    border-radius: 32px 0 0 32px;
  }
  &-right {
    border-radius: 0 32px 32px 0;
  }
}
.container {
  box-shadow: 10px 15px 25px 0px rgba(0,0,0,0.1);
  max-width: 800px;
  border-radius: 32px;
}
.product-subtitle {
  letter-spacing: 8px;
}
.product-title {
  font-size: 42px;
  font-weight: 700;
  line-height: 1;
}
.product-description {
  font-size: 18px;
  line-height: 1.5;
}
.price {
  font-size: 42px;
  font-family: 'Fraunces', serif;

  &--small {
    font-size: 18px;
  }
  &--color {
   color: hsl(158, 36%, 37%);
  }
}
.opacity-6 {
  opacity: 0.6;
}
</style>
