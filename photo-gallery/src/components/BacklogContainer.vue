<template>

  <ion-fab slot="fixed" vertical="bottom" horizontal="center">
    <ion-button id="open-modal" expand="block" shape="round">
      <p>Recomendador</p>
    </ion-button>
  </ion-fab>

  <AddGame />

  <ion-row class="ion-padding-horizontal" style="width: max-content;">
    <ion-chip color="primary">   
      <ion-label>All</ion-label>
      <!-- <ion-icon :icon="closeCircle"></ion-icon> -->
    </ion-chip>
    <ion-chip :outline="true">Nintendo</ion-chip>
    <ion-chip :outline="true">PlayStation</ion-chip>
    <ion-chip :outline="true">Xbox</ion-chip>
    <ion-chip :outline="true">PC</ion-chip>
  </ion-row>

  <div id="container">
    <!--  -->
    <ion-list>

      <ion-grid>
        <ion-row>
          <ion-col>
            <ion-nav-link router-link="/detail">
              <ion-card class="ion-no-margin">
                <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
                <ion-card-header>
                  <ion-card-title>Card Title</ion-card-title>
                  <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
                </ion-card-header>

                <!-- <ion-card-content>
                  Here's a small text description for the card content. Nothing more, nothing less.
                </ion-card-content> -->
              </ion-card>
            </ion-nav-link>
          </ion-col>
          <ion-col>
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <!-- <ion-col>3</ion-col> -->
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <!-- <ion-col>3</ion-col> -->
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <!-- <ion-col>3</ion-col> -->
        </ion-row>
        <ion-row>
          <ion-col size="6">
            <ion-card class="ion-no-margin">
              <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
              <ion-card-header>
                <ion-card-title>Card Title</ion-card-title>
                <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
              </ion-card-header>

              <!-- <ion-card-content>
                Here's a small text description for the card content. Nothing more, nothing less.
              </ion-card-content> -->
            </ion-card>
          </ion-col>
          <!-- <ion-col>3</ion-col> -->
        </ion-row>
      </ion-grid>

    </ion-list>
    <!-- / -->
  </div>

</template>

<script setup lang="ts">
import { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle } from '@ionic/vue';
import { IonHeader, IonTitle, IonToolbar, IonContent, IonNavLink, IonButton } from '@ionic/vue';
import { markRaw } from 'vue';
import detail from '../views/detail.vue';
import AddGame from '../components/AddGame.vue';
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
