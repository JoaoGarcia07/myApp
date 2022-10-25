<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Avião Do Toguro</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <di class="conteudo">
       <h1>Em pleno 2022 Pai?</h1>
       <h2>LOCÃo DE PRÉ TREINO</h2>
    </di>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';


export default defineComponent({
  name: 'Tab2Page',
  components: {  IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>

<style>
h1{
  color: rgb(157, 0, 255);
}
h2{
  color: rgb(119, 0, 255);
}
.conteudo {
  display: flex;
  align-items: center;
  justify-content: center;

}

</style>