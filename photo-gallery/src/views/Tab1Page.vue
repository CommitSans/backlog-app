<template>
  <ion-page>

    <!-- -->
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Backlog</ion-title>
        <ion-buttons :collapse="true" slot="end">
          <ion-button>
            <ion-icon slot="icon-only" :icon="personCircle"></ion-icon>
          </ion-button>
          <ion-button>
            <ion-icon slot="icon-only" :icon="personCircle"></ion-icon>
          </ion-button>
          <ion-button>
            <ion-icon slot="icon-only" :icon="personCircle"></ion-icon>
          </ion-button>
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
            <ion-button>
              <ion-icon slot="icon-only" :icon="createOutline"></ion-icon>
            </ion-button>
            <ion-button>
              <ion-icon slot="icon-only" :icon="addCircleOutline"></ion-icon>
            </ion-button>
            <ion-button>
              <!-- <ion-icon slot="icon-only" :icon="personCircle"></ion-icon> -->
              <ion-avatar>
                <img alt="Silhouette of a person's head" src="https://pbs.twimg.com/profile_images/1661688257938087936/DzSsGyeO_400x400.jpg" />
              </ion-avatar>
            </ion-button>
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
import { defineComponent } from 'vue';
import { create, ellipsisHorizontal, ellipsisVertical, helpCircle, personCircle, createOutline, addCircleOutline, pencilOutline, search, star } from 'ionicons/icons';
import BacklogContainer from '@/components/BacklogContainer.vue';
</script>
