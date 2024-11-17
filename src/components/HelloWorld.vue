<template>
    <div>
        <h2>Мой компонент</h2>
        <button @click="toggleText">{{ showText ? 'Скрыть' : 'Показать' }}</button>
        <!-- <button @click="showText = !showText">{{ showText ? 'Скрыть' : 'Показать' }}</button> -->
        <p v-show="showText">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur fugit a ducimus totam minima esse voluptates eos repellendus nesciunt pariatur nobis placeat rem ipsa animi quidem, fugiat reprehenderit in exercitationem.</p>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const showText = ref(false);
const toggleText = () => {
    showText.value = !showText.value
}

</script>

<style lang="scss" scoped>

</style>