<template>
  <div>
    <NavbarVue />
    <h1>Criar novo pedido</h1>
    <v-form>
      <v-container>
        <v-row>
          <v-text-field v-model="pedido.cliente.nome" label="Nome do cliente" />
          <v-text-field v-model="pedido.cliente.telefone" label="Telefone do cliente" />
          <v-text-field v-model="pedido.cliente.endereco" label="Endereço do cliente"/>
          <v-text-field v-model="pedido.cliente.logradouro" label="Logradouro do cliente"/>
          <v-text-field v-model="pedido.cliente.numero" label="Número do cliente"/>
          <v-text-field v-model="pedido.cliente.bairro" label="Bairro do cliente"/>
          <v-text-field v-model="pedido.cliente.complemento" label="Complemento do cliente"/>
          <v-text-field v-model="pedido.cliente.referencia" label="Referência do cliente"/>
        </v-row>
      </v-container>
    </v-form>
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
      pedido: {
        cliente: {
          nome: "",
          telefone: "",
          endereco: {
            logradouro: "",
            numero: "",
            bairro: "",
            complemento: "",
            referencia: ""
          }
        },
        listaProdutos: [],
        valorTotal: 0,
        formaPagamento: ""
      }
    }
  }
}
</script>
<style>
  
</style>
