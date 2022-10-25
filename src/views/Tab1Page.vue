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

    <ion-button fill="outline" shape="round" @click="exibirTexto()">
      <ion-icon :icon="add"></ion-icon>
    </ion-button>
    </ion-content>
  </ion-page>
</template>


<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent,alertController } from '@ionic/vue';
import {add} from  "ionicons/icons";

export default  defineComponent({
  name: 'Tab1Page',
  components: {  IonHeader, IonToolbar, IonTitle, IonContent, IonPage },
  setup(){
    const exibirTexto = async () => {
      const alert = await alertController.create({
        header: 'Clique do Botão',
        subHeader:'',
        message:'Voce acabou de utilizar o alert do android ou IOS',
        buttons:['Entendido'],
      });
     
    await alert.present();

    };
    return{
      add,
      exibirTexto
    }
  },
  exibirTuxto(){
    console.log("TEste do onclick");
  },
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

ion-button {
    --background: #535353;
    --background-hover: #222524;
    --background-activated: #8f8f8f;
    --background-focused: #ffffff;

    --color: blue;

    --border-radius: 360px;
    --border-color: #000;
    --border-style: solid;
    --border-width: 1px;

    --box-shadow: 0 2px 6px 0 rgb(0, 0, 0, 0.25);

    --ripple-color: deeppink;

    --padding-top: 10px;
    --padding-bottom: 10px;
  }

</style>