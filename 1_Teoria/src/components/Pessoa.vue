<template>
    <div>
        <h2>Descrição da pessoa: {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando=false />
        <Form />        
    </div>
</template>

<script>
import Info from './Info.vue'
import Form from './form/Form.vue'

export default {
    name: 'Pessoa',
    components: {
        Info,
        Form
    },
    
    data() {
        return {
            nome: 'Eu',
            email: 'leandro@email.com'
        }
    }    
}
</script>