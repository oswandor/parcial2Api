<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>API Fetch</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Api Fetch</ion-title>
        </ion-toolbar>
      </ion-header>



      <NewFecth></NewFecth>


    </ion-content>

    <ion-footer :translucent="true">
      <ion-toolbar>
        <ion-title>Ronal Gonzalez</ion-title>
      </ion-toolbar>
    </ion-footer>


  </ion-page>
</template>

<script setup>
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import NewFecth from './NewFecth.vue';
</script>
