<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>HFFI Map</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content class="ion-padding">
      <MarkerMap></MarkerMap>
      <ion-button style="position: absolute; bottom: 50%; width: 100px"></ion-button>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonButton, IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import { defineComponent } from 'vue';
import MarkerMap from '@/components/marker-map.vue';

export default defineComponent({
  name: 'MapPage',
  components: {
    IonButton,
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    MarkerMap,
  },
});
</script>

<style scoped></style>
