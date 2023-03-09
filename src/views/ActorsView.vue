<template>
    <div>
        <h1>Movies</h1>
        <div class="flex flex-wrap justify-around">
            <actorcard />
            <actorcard />
            <actorcard />
            <actorcard />
            <actorcard />
            <actorcard />
            <actorcard />
            <actorcard />
        </div>
    </div>
</template>
<script>
import actorcard from '../components/actorcard.vue';
export default {
    components: {
        actorcard
    }
}
</script>