<template >
  <nav>
    <router-link to="/"></router-link> 
  </nav>
  <router-view/>
</template>

<style>

  #app{
    background: linear-gradient(to bottom, #009B3A, #FFD700);
    /* Para navegadores que não suportam gradientes */
    background-color: #009B3A;
  }

* {
  
    margin: 0;
    padding: 0;
    box-sizing: border-box; /* Isso garante que o tamanho total de um elemento inclua a borda e o preenchimento, não apenas o conteúdo */
}

</style>
