<template>
    <div>    
        <button type="button" class="text-left block w-full border border-blue-800 relative px-6 py-4 rounded mb-4"
            :class="[ selected ? 'bg-blue-800' : 'opacity-50 hover:opacity-100 hover:bg-blue-800' ]"
        >
            <div v-show="selected" class="absolute -ml-10 py-6 flex items-center">
                <svg class="h-6 w-6 fill-current text-gray-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M256 8C119.033 8 8 119.033 8 256s111.033 248 248 248 248-111.033 248-248S392.967 8 256 8zm0 48c110.532 0 200 89.451 200 200 0 110.532-89.451 200-200 200-110.532 0-200-89.451-200-200 0-110.532 89.451-200 200-200m140.204 130.267l-22.536-22.718c-4.667-4.705-12.265-4.736-16.97-.068L215.346 303.697l-59.792-60.277c-4.667-4.705-12.265-4.736-16.97-.069l-22.719 22.536c-4.705 4.667-4.736 12.265-.068 16.971l90.781 91.516c4.667 4.705 12.265 4.736 16.97.068l172.589-171.204c4.704-4.668 4.734-12.266.067-16.971z"/></svg>
            </div>
            <div class="flex items-center -mx-4">
                <div class="px-4 w-2/5 text-gray-400">
                    <h2 class="text-xl font-semibold mb-2">{{ name }}</h2>
                    <div class="font-semibold">
                        <span class="text-3xl font-bold">${{ monthly }}</span>
                        <span class="mx-1">/</span>
                        <span>Month</span>
                    </div>
                </div>
                <div class="px-4 w-3/5 text-sm text-gray-500 font-semibold">
                    <ul class="">
                        <li v-bind:key="feature" v-for="(feature, i) in features" :class="[ i === features.lenght - 1 ? '' : 'mb-1' ]">{{ feature }}</li>
                    </ul>
                </div>
            </div>
        </button>
    </div>
</template>

<script>
export default {
    props: [
        'name',
        'monthly',
        'selected',
        'features',
    ],
    data() {
        return {

        }
    },
    methods: {

    },
}
</script>

<style>

</style>