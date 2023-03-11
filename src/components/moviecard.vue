<template>
    <div class="bg-gray-900 max-w-sm m-11 rounded overflow-hidden shadow-lg">
        <img class="w-full" :src="image" alt="Movie Poster">
        <div class="px-6 py-4">
            <div class="font-bold text-white  text-xl mb-2">{{ name }}</div>
            <p class="text-white text-base">{{ description }}</p>
        </div>
        <div class="px-6 py-4">
            <span
                class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">#Tag1</span>
            <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700">#Tag2</span>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        name: String,
        description: String,
        image: String,
    },
}
</script>