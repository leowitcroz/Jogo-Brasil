<template>
  <div class="tela" style="height: 100vh; ba">
    <div class="hello">
      <div class="main">
        <h1 class="text">Quer Assistir o Jogo Do Brasil De Casal Comigo?</h1>
        <div class="buttons">
          <button class="butao" @click="simOuNao = true">SIM</button>
          <button class="butao" @click="simOuNao = false">NÃO</button>
        </div>

        <div class="casos">
          <p v-if="simOuNao" class="textoGatinho">Uhuuuu... Ja Que Insiste... Te Amo</p>
          <p v-else class="textoGatinho">Resposta Errada Tente Novamente!</p>
          <img v-if="simOuNao" class="gatinhoNao" src="../assets/Slash.jpg" alt="">
          <img v-else class="gatinhoNao" src="../assets/gatinBravo.png" alt="">
        </div>
      </div>
    </div>
  </div>

</template>

<script lang="ts" setup>
import { onMounted, ref } from 'vue';

const simOuNao = ref()



</script>


<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  /* Isso garante que o tamanho total de um elemento inclua a borda e o preenchimento, não apenas o conteúdo */
}

@media only screen and (max-width: 991px) {


  .hello {
    padding-top: 30%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .textoGatinho {
    color: white;
    font-size: 23px;
  }

  .casos {
    flex-direction: column;
    margin-top: 5%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .gatinhoNao {
    margin-top: 5%;
    width: 65%;
  }

  .text {
    text-align: center;
    font-size: 33px;
    color: white;
    font-weight: 600;
  }

  .buttons {
    display: flex;
    justify-content: center;
  }


  .butao {
    margin: 5%;
    font-family: Roboto, sans-serif;
    font-weight: 0;
    font-size: 14px;
    color: #fff;
    background: linear-gradient(90deg, #1e7cd9 0%, #3a535e 100%);
    padding: 10px 30px;
    border: none;
    border-radius: 50px;
    cursor: pointer;
  }

  .butao:hover {
    background: linear-gradient(90deg, #1e7cd9 0%, #264653 100%);
    border: solid 2px #0066cc;
  }
}
</style>