<script setup>
alert("Alumna: Evelin Itzel Arias Vasquez" + "\n" + "Materia: Aplicaciones Web Orientadas a servicios" +  "\n" + "4° A");
</script>

<template>
        
      <div class="containercontent text-center mt-5">
    <img src="./assets/logo.svg" alt="" srcset="" widht="125" height="125" class="m-2">
    <h1 class="text-center text-danger">Hola desde vue.js 3</h1>
    <hr>
  <div class="m-1 text-center">
   <h2 class="text-light">Contador {{contador}}</h2>
   <button class="btn btn-light m-1" @click="incrementar()">+1</button>
   <button class="btn btn-danger m-1" @click="disminuir()">-1</button>
   <button class="btn btn-primary m-1" @click="reset()">Reset</button>
  </div>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
<script>
export default{
    data:() =>({
     contador : 500,
    }),
    methods:{
      incrementar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      reset(){
        this.contador = 500;
      },
    },
  };
</script>