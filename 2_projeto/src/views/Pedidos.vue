<template>
  <section class="pedidos">
    <h1>Gerenciar pedidos:</h1>
    <Dashboard />
  </section>
</template>

<script>
import Dashboard from '../components/Dashboard.vue'

export default {
  name: "Pedidos",

  components: {
    Dashboard
  }
}

</script>

<!-- {
      "nome": "landing page",
      "pao": "3 Queijos",
      "carne": "Maminha",
      "opcionais": [
        "Salame",
        "Bacon",
        "Tomate"
      ],
      "status": "Solicitado",
      "id": 1
    },
    {
      "nome": "landing page",
      "pao": "3 Queijos",
      "carne": "Maminha",
      "opcionais": [
        "Salame",
        "Bacon",
        "Tomate"
      ],
      "status": "Solicitado",
      "id": 2
    } -->