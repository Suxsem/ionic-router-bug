<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>SubTab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">SubTab 1</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-button @click="router.push('/tabs/tab1/subtab1')">Go to subtab1</ion-button>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import { useRouter } from "vue-router";

export default  {
  name: 'SubTab1',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage },
  setup() {
    const router = useRouter();
    return {
      router
    };
  }
}
</script>