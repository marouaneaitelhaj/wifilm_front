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
    mounted() {
        axios.get('http://127.0.0.1:8000/api/movies', {
            headers: {
                "Authorization": `Bearer ${this.$root.token}`
            }
        })
            .then(response => {
                console.log(response.data)
                this.movies = response.data
            })
            .catch(error => {
                console.log(error)
            })
    },
}
</script>