<template>
    <div>
        <h1>Movies</h1>
        <div class="flex flex-wrap justify-around">
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
            <MovieCard />
        </div>
    </div>
</template>
<script>
import MovieCard from '@/components/movieCard.vue'
export default {
    components: {
        MovieCard
    }
}
</script>