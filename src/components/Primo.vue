<template>
  <div>
  
   <div class="mt-3">
    <b-card-group deck>
      <b-card bg-variant="dark" header="Primo" text-variant="white" class="text-center">
        <b-card-text>{{ calcular_primo(numero) }}</b-card-text>
      </b-card>
    </b-card-group>
  </div>
  </div>
</template>

<script>
export default {
  name: 'Primo',
  props:{
    numero: Number
  },
  methods:{
    calcular_primo(n){
      return n **3
    }
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
