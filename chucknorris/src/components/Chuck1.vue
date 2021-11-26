<template>
 <div id="app">
          <div id="ImgChuck">
            <img  width="100" height="100" src="../assets/Norris.jpg" alt="Chuck">
          </div>
        
          <h1>CHUCK NORRIS CONVERTER</h1>
          <label class="col-sm-2 col-form-label"><b>Ingrese un numero:</b> </label><br>
          <input id="name" v-model="message"> 
          <button v-on:click="myFunctionClick" class="btn btn-success btn-primary" data-bs-toggle="button" autocomplete="off">
            Convertir
          </button>
          
          <div>
            <br>
            <ol>
              <li><b>Caracter:</b> {{dato}}</li>
              <li><b>Decimal:</b> {{asciiCode}}</li>
              <li><b>Hexa:</b> {{hexValue}} </li>
              <br>
              <li><b>Binario:</b> {{NumeroFull}} </li>
              <li><b>Chuck Norris:</b> </li>
            </ol>

            </div>
  </div>
</template>

<script>
export default {
  name: 'Chuck1',
  data:()=>({
    Binario : 0,
    dato:0,
    asciiCode:0,
    hexValue:0,
    NumeroFull:[],
    Numero:0
  }),
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
