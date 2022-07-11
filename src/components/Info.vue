<template>
    <div>
        <p v-if="esta_trabalhando">Esta pessoa está trabalhando.</p>
        <p v-else>Esta pessoa NÃO está trabalhando</p>
        <button v-on:click="workToggle">Toggle Work</button>
        <ul>
            <li>PHP</li>
            <li>Python</li>
            <li>JavaScript</li>
        </ul>
        <p>Portifólio da pessoa: <a v-bind:href="meu_link" target="_blank">Clique Aqui.</a></p>
    </div>
</template>

<script>

export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: true,
            meu_link: "https://google.com"
        }
    },
    methods: {
        workToggle() {
            if (this.esta_trabalhando === true) this.esta_trabalhando = false;
            else this.esta_trabalhando = true;
        },
    }
}
</script>