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
    <img alt="Silhouette of mountains" src="https://cdn2.steamgriddb.com/thumb/425bba74301311395421f24f0b2205d3.jpg" />
    <ion-content class="ion-padding">
      <h1>Cuphead</h1>
      <p>Descripción</p>
      <ion-button expand="block">Hacer algo</ion-button>
    </ion-content>
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