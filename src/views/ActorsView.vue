<template>
    <div>
        <h1>Movies</h1>
        <div class="flex flex-wrap justify-around">
            <div v-for="actor in actors">
                <actorcard :name="actor.name" :description="actor.description" :image="actor.image" />
            </div>
        </div>
    </div>
</template>
<script>
import actorcard from '../components/actorcard.vue';
export default {
    components: {
        actorcard
    },
    data() {
        return {
            actors: []
        }
    },
}
</script>