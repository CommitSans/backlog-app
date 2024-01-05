<template>

  <ion-fab slot="fixed" vertical="bottom" horizontal="end">
    <ion-fab-button>
      <ion-icon :icon="add"></ion-icon>
    </ion-fab-button>
  </ion-fab>

  <ion-row class="ion-padding-horizontal" style="width: max-content;">
    <ion-chip :outline="true">Platform</ion-chip>
    <ion-chip color="success">   
      <ion-label>Not started</ion-label>
      <ion-icon :icon="closeCircle"></ion-icon>
    </ion-chip>
    <ion-chip :outline="true">Studio</ion-chip>
    <ion-chip color="success">Platformer</ion-chip>
    <ion-chip :outline="true">Default</ion-chip>
    <ion-chip :outline="true">Default</ion-chip>
  </ion-row>

  <div id="container" style="margin-top: 16px;">
    <!--  -->
    <ion-nav-link router-link="/detail">
      <ion-card style="margin-top: 0;">
        <img alt="Silhouette of mountains" src="https://cdn2.steamgriddb.com/thumb/425bba74301311395421f24f0b2205d3.jpg" />
        <ion-card-header>
          <ion-card-title>Cuphead</ion-card-title>
          <ion-card-subtitle>Nintendo Switch · Steam</ion-card-subtitle>
        </ion-card-header>
        <ion-card-content>
          <!-- <p>Here's a small text description for the card content. Nothing more, nothing less.</p> -->
        </ion-card-content>
      </ion-card>
    </ion-nav-link>
    <!-- / -->
    <!--  -->
    <ion-card>
      <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
      <ion-card-header>
        <ion-card-title>Card Title</ion-card-title>
        <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
      </ion-card-header>

      <ion-card-content>
        Here's a small text description for the card content. Nothing more, nothing less.
      </ion-card-content>
    </ion-card>
    <!-- / -->
    <!--  -->
    <ion-card>
      <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
      <ion-card-header>
        <ion-card-title>Card Title</ion-card-title>
        <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
      </ion-card-header>

      <ion-card-content>
        Here's a small text description for the card content. Nothing more, nothing less.
      </ion-card-content>
    </ion-card>
    <!-- / -->
  </div>

</template>

<script setup lang="ts">
import { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle } from '@ionic/vue';
import { IonHeader, IonTitle, IonToolbar, IonContent, IonNavLink, IonButton } from '@ionic/vue';
import { markRaw } from 'vue';
import detail from '../views/detail.vue';
import { IonChip, IonAvatar, IonLabel, IonIcon } from '@ionic/vue';
import { add, close, closeCircle, pin } from 'ionicons/icons';
</script>

<style scoped>
#container {
  left: 0;
  right: 0;
  top: 50%;
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
