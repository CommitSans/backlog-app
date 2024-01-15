<template>
  <ion-header>
    <ion-toolbar>
      <!-- <ion-buttons slot="start">
        <ion-back-button></ion-back-button>
      </ion-buttons> -->
      <ion-buttons slot="start">
        <ion-button>Back</ion-button>
      </ion-buttons>
      <!-- <ion-title>Cuphead</ion-title> -->
    </ion-toolbar>
  </ion-header>

  <ion-content>
    <ion-img
      src="https://cdn2.steamgriddb.com/hero_thumb/5988319f8fdeb1b2d254a9a38518f52e.jpg"
      alt="The Wisconsin State Capitol building in Madison, WI at night"
    ></ion-img>
    <ion-img
      src="https://cdn2.steamgriddb.com/thumb/4030e2eebb977639f8836aa25a293e40.jpg"
      alt="The Wisconsin State Capitol building in Madison, WI at night"
    ></ion-img>
  </ion-content>

</template>

<script lang="ts">
  import { markRaw } from 'vue';
  import {
    IonHeader,
    IonTitle,
    IonToolbar,
    IonContent,
    IonNavLink,
    IonButton,
    IonButtons,
    IonBackButton,
  } from '@ionic/vue';
  import PageThree from './PageThree.vue';

  export default {
    components: {
      IonHeader,
      IonTitle,
      IonToolbar,
      IonContent,
      IonNavLink,
      IonButton,
      IonButtons,
      IonBackButton,
    }
  };
</script>