<template>
    <img :src="props.tweet.user.image" class="profile" alt="profile" />
</template>
<script setup>
import {defineProps} from 'vue';

const props = defineProps({
    image:String
    })


</script>
<style scoped>
</style>