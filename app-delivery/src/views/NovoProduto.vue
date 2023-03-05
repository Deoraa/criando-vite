<template>
  <div>
    <NavbarVue />
    <h1>Criar novo produto</h1>
    <v-container>
      <v-row>
        <v-text-field v-model="produto.nome" label="Nome do produto" />
        <v-text-field v-model="produto.valor" type="number" label="Valor do produto" />
      </v-row>
    </v-container>
    <v-btn color="green" @click="cadastrarProduto">Cadastrar</v-btn>
  </div>
</template>

<script>
import NavbarVue from '../components/Navbar.vue'
export default {
  components: {
    NavbarVue
  },
  data(){
    return {
      produto: {
        nome: "",
        valor: 0
      }
    }
  },
  methods: {
    cadastrarProduto(){
      alert(this.produto.nome)
    }
  }
}
</script>
<style>
  
</style >