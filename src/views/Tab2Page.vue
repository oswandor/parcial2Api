<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Axios</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Axios</ion-title>
        </ion-toolbar>
      </ion-header>

      <APIMorty />
    </ion-content>

    
  </ion-page>
</template>

<script setup>
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import APIMorty from './APIMorty.vue';
</script>
