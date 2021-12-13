<template>
    <h1>hello</h1>
    <p class="capitalize">{{ name }}</p>
</template>
<script setup>
import { computed } from 'vue'
import { useStore } from 'vuex'
const store = useStore()

const name = computed(() => {
    return store.state.user.name
})
</script>
