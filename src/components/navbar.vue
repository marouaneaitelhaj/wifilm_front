<template>
    <header aria-label="Site Header" class="shadow-sm bg-black">
        <div class="mx-auto flex h-16 max-w-screen-xl items-center justify-between px-4">
            <div class="flex w-0 flex-1 lg:hidden">
                <button class="rounded-full bg-gray-100 p-2 text-gray-600" type="button">
                    <span class="sr-only">Account</span>
                    <svg class="h-5 w-5" fill="none" stroke="currentColor" viewbox="0 0 24 24"
                        xmlns="http://www.w3.org/2000/svg">
                        <path d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" stroke-linecap="round"
                            stroke-linejoin="round" stroke-width="2"></path>
                    </svg>
                </button>
            </div>

            <div class="flex items-center gap-4">
                <a href="#">
                    <span class="sr-only">Logo</span>
                    <span class="h-10 w-20 rounded-lg bg-gray-200"></span>
                </a>

                <form class="mb-0 hidden lg:flex">
                    <div class="relative">
                        <input class="h-10 rounded-lg border-gray-200 pr-10 text-sm placeholder-gray-300 focus:z-10"
                            placeholder="Search..." type="text" />

                        <button type="submit" class="absolute inset-y-0 right-0 rounded-r-lg p-2 text-gray-600">
                            <span class="sr-only">Submit Search</span>
                            <svg class="h-5 w-5" fill="currentColor" viewbox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                <path clip-rule="evenodd"
                                    d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                                    fill-rule="evenodd"></path>
                            </svg>
                        </button>
                    </div>
                </form>
            </div>

            <div class="flex w-0 flex-1 justify-end lg:hidden">
                <button class="rounded-full bg-gray-100 p-2 text-gray-500" type="button">
                    <span class="sr-only">Menu</span>
                    <svg class="h-5 w-5" fill="currentColor" viewbox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                        <path clip-rule="evenodd"
                            d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                            fill-rule="evenodd"></path>
                    </svg>
                </button>
            </div>

            <nav aria-label="Site Nav"
                class="hidden items-center justify-center gap-8 text-sm font-medium lg:flex lg:w-0 lg:flex-1">
                <RouterLink class="flex-shrink-0 pl-4 text-white" to="./">Home</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-white" to="Movies">Movies</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-white" to="Actors">Actors</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-white" to="About">About</RouterLink>
            </nav>
            <div class="hidden items-center gap-4 lg:flex">
                <RouterLink to="login" class="rounded-lg bg-white px-5 py-2 text-sm font-medium text-black">
                    Log in
                </RouterLink>

                <RouterLink to="signup"
                    class="rounded-lg bg-black border-2 border-solid border-white px-5 py-2 text-sm font-medium text-white">
                    Sign up
                </RouterLink>
            </div>
        </div>

        <div class="border-t border-gray-100 lg:hidden">
            <nav class="flex items-center justify-center overflow-x-auto p-4 text-sm font-medium">
                <RouterLink class="flex-shrink-0 pl-4 text-gray-900" to="./">Home</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-gray-900" to="Movies">Movies</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-gray-900" to="Actors">Actors</RouterLink>
                <RouterLink class="flex-shrink-0 pl-4 text-gray-900" to="About">About</RouterLink>
            </nav>
        </div>
    </header>
</template>
<script>
import { RouterLink, RouterView } from 'vue-router'
export default {
    name: 'Navbar'
}
</script>