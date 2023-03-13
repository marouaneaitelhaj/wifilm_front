<template>
    <div>
        <h1>Movies</h1>
        <div class="flex flex-wrap justify-around">
            <div v-for="movie in movies">
                <MovieCard :name="movie.name" :description="movie.description" :image="movie.image" />
            </div>
        </div>
    </div>
</template>
<script>
import MovieCard from '@/components/movieCard.vue'
export default {
    components: {
        MovieCard
    },
    data() {
        return {
            movies: []
        }
    },
    
}
</script>