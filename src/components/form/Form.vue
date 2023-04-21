<template>
    <form action="">
        <div>
            <InputText />
            <InputText />
            <Submit />
        </div>
    </form>
</template>

<script>
import InputText from "./InputText.vue"
import Submit from "./Submit.vue"
export default {
    name: 'Form',
    components: {
        InputText,
        Submit
    }
}
</script>