<template>
  <div>
    <div class="w-48 flex bg-blue-800 text-gray-500 rounded mb-4 overflow-hidden mx-auto h-6">
        <button @click="select('monthly')" 
            type="button" class="py-1 rounded uppercase text-center w-1/2 text-xs font-bold tracking-wide"
            :class="[isMonthly ? 'bg-white text-gray-900' : 'hover:text-white hover:bg-blue-700']"    
        >
            Monthly
        </button>
        <button @click="select('yearly')" 
            type="button" class="py-1 rounded uppercase text-center w-1/2 text-xs font-bold tracking-wide"
            :class="[isYearly ? 'bg-white text-gray-900' : 'hover:text-white hover:bg-blue-700']"    
        >
            Yearly
        </button>
    </div>
  </div>
</template>

<script>
export default {
    props: ['value'],
    computed: {
        isMonthly() {
            return this.value === 'monthly'
        },
        isYearly() {
            return this.value === 'yearly'
        }
    },
    methods: {
        select() {

        }
    }
}
</script>

<style>

</style>