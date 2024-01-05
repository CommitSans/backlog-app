<template>
  <ion-page>

    <!-- -->
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Backlog</ion-title>
        <ion-buttons :collapse="true" slot="end">
          <ion-button>Edit</ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <!-- / -->

    <ion-content :fullscreen="true">
      <!--  -->
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Backlog</ion-title>
          <ion-buttons :collapse="true" slot="end">
            <ion-button>Edit</ion-button>
          </ion-buttons>
        </ion-toolbar>
      </ion-header>
      <!-- / -->

      <BacklogContainer name="Backlog" />
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import BacklogContainer from '@/components/BacklogContainer.vue';
</script>
