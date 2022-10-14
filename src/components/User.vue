<template>
    <span class="user">
        <span class="user">
        <span class="name">{{props.tweet.user.name}}</span>
        <span class="handle">@{{props.tweet.user.handle}}</span>
    </span>
</template>
<script setup>
import {defineProps} from 'vue'

const props = defineProps({
    name: String,
    handle: String
})
</script>
<style scoped>
</style>