<template>
    <div class="tweet">
        <ProfileImage :image="props.tweet.user.image" />
        <div class="body">
            <div class="top">
                <User :name="props.tweet.user.name" :handle="props.tweet.user.handle" />

                <Timestamp :timestamp="props.tweet.timestamp" />
            </div>
            <Message :message="props.tweet.message" />
            <Actiions :actions="props.twwet.actions" />
        </div>

        <i class="fas fa-ellipsis-h"></i>
    </div>
</template>
<script setup>
import { defineProps } from 'vue'
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'
import Timestamp from './Timestamp.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

const props = defineProps({
    tweet: Object
})
</script>

<style scoped>
a {
    color: #42b983;
}
</style>
