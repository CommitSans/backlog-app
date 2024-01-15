<template>
  <ion-content class="ion-padding">

    <div class="ion-padding ion-align-items-center" style="display: flex; flex-direction: column; width: 100%;">
      <ion-avatar>
        <img alt="Silhouette of a person's head" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
      </ion-avatar>

      <ion-label>
        <h1>Carlos Lorca</h1>
      </ion-label>
    </div>

    <ion-list>
      <ion-item>
        <ion-icon aria-hidden="true" :icon="airplane" slot="start"></ion-icon>
        <ion-label>Settings</ion-label>
      </ion-item>
      <ion-item>
        <ion-icon aria-hidden="true" :icon="wifi" slot="start"></ion-icon>
        <ion-label>Share with friends</ion-label>
      </ion-item>
      <ion-item>
        <ion-icon aria-hidden="true" :icon="bluetooth" slot="start"></ion-icon>
        <ion-label>Get in touch</ion-label>
      </ion-item>
      <ion-item>
        <ion-icon aria-hidden="true" :icon="call" slot="start"></ion-icon>
        <ion-label>Donate</ion-label>
      </ion-item>
      <ion-item>
        <ion-icon aria-hidden="true" :icon="call" slot="start"></ion-icon>
        <ion-label>Log out</ion-label>
      </ion-item>
    </ion-list>

  </ion-content>
</template>

<script setup lang="ts">
defineProps({
  name: String,
});
import { defineComponent } from 'vue';
  import { airplane, bluetooth, call, wifi } from 'ionicons/icons';
</script>

<style scoped>

</style>
