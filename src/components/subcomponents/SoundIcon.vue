<script>
    export default { 
        data() {
            return {
                soundEmojis: ['🔇', '🔈', '🔉', '🔊']
            }
        },
        props: {
            soundLevel: Number
        }
    }
</script>

<template>
    <!-- TODO: add your template code here. Use span element. --> 
    <span>{{soundEmojis[soundLevel]}}</span>
</template>