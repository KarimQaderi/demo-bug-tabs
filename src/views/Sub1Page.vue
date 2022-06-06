<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Sub 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Sub 1</ion-title>
        </ion-toolbar>
      </ion-header>

        <div style="padding: 20px" @click="$router.push('/sub/two')">Sub 2 Page</div>

    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';

export default  defineComponent({
  name: 'Sub1Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>
