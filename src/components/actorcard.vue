<template>
    <div class="bg-gray-900 max-w-sm m-11 rounded overflow-hidden shadow-lg">
        <img class="w-full h-64 object-cover" :src="image" alt="Actor's name">
        <div class="px-6 py-4">
            <h2 class="text-xl text-white font-bold mb-2">{{ name }}</h2>
            <p class="text-white text-base">Born: January 1, 1970<br>Age: 53<br>Birthplace: City, Country</p>
            <p class="text-white text-base mt-4">{{ description }}</p>
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