<script>
export default{
  data: ()=> ({
  contador: 10,
  }),
  methods: {
    incrementar(){
     this.contador++;
    },
    disminuir(){
      this.contador--;
    },
    reset(){
      this.contador=10;
    },
  },
};

</script>
<template>
  <div class="container">
  <img src="./assets/logo.svg" alt="logo vue" width="125" height="125">
  <small>
    <h1>hola mundo sesde vuejs3</h1>
  </small>
  <hr/>
  <h2>contador: {{ contador }}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="disminuir()">-1</button>
  <button @click="reset()">reset</button>

  </div>
</template>

<style scoped>
.container {
text-align: center;
}
h1 {
  font-weight: bolder;
}
small {
  color: #666;
}
h2{
  font-size: 2.5rem;
}
button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}

</style>