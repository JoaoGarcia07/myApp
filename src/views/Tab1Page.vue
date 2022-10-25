<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Foguete do Elon</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
    <di class="conteudo">
       <h1>Conhece Elon musk pai?</h1>
       <h2>Ta fazendo um foguete</h2>
    </di>
    </ion-content>
  </ion-page>
</template>


<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';


export default  defineComponent({
  name: 'Tab1Page',
  components: {  IonHeader, IonToolbar, IonTitle, IonContent, IonPage },
  ionViewDidEnter(){
    console.log('Entrou na página');
  },
  ionViewDidLeave(){
    console.log('Saiu na página');
  },
  ionViewWillEnter(){
    console.log('Vai entrar na página');
  },
  ionViewWillLeave(){
    console.log('Vai sair da página');
  },
});
</script>

<style scoped="style">
h1{
  color: orange;
}
h2{
  color: orange;
}
.conteudo {
  text-align: center;

  
}

</style>