<template>
  <GoogleMap
    api-key="AIzaSyB5Ni6fBoDWDDAMKI_nqplDxflaXXnGKdE"
    style="width: 100%; height: 500px"
    :center="center"
    :zoom="zoom"
  >
    <Marker :options="{ position: center, icon: '@/assets/red-house-icon.png' }" />
  </GoogleMap>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { GoogleMap, Marker } from 'vue3-google-map';

export default defineComponent({
  components: { GoogleMap, Marker },

  setup() {
    const center = { lat: 38.003343, lng: -77.3434343 };
    const zoom = 10;
    const labelText = 'X';
    const icon = '@resources/red-house-icon.png';

    return { center, zoom };
  },
});
</script>

<style scoped>
.map-frame {
  width: 100%;
  height: 300px;
  background-color: azure;
}
</style>
