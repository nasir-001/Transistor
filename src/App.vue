<template>
  <div id="app" class="antialiased leading-tight">
    <div class="container mx-auto px-8">
      <header class="flex justify-between py-6 items-center">
        <div>
          <svg class="block h-12 fill-current text-gray-400 border-2 border-gray-400 px-4 py-4 rounded-full" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M416 208H272V64c0-17.67-14.33-32-32-32h-32c-17.67 0-32 14.33-32 32v144H32c-17.67 0-32 14.33-32 32v32c0 17.67 14.33 32 32 32h144v144c0 17.67 14.33 32 32 32h32c17.67 0 32-14.33 32-32V304h144c17.67 0 32-14.33 32-32v-32c0-17.67-14.33-32-32-32z"/></svg>
        </div>
        <div>
            <a class="font-medium text-gray-400 hover:underline" href="#">Sign in</a>
        </div>
      </header>
      <div class="pt-16 pb-16">
          <h1 class="text-gray-400 text-center font-normal text-2xl sm:text-3xl pb-16">Start your podcast today:</h1>
          <div class="flex flex-wrap -mx-4">
              <div class="w-full md:w-1/2 px-4 pt-10">
                <plan-selector></plan-selector>
              </div>
              <div class="w-full md:w-1/2 px-4 mb-6 md:mb-0 md:pt-10">
                <div class="pb-8">
                    <form action="#" method="POST" class="">
                        <h1 class="md:hidden text-center text-white text-2xl text-medium mb-4">Your Information</h1>
                        <input placeholder="Your Name" class="text-white text-xl text-center focus:bg-blue-700 font-medium block  w-full bg-blue-800 px-4 py-4 mb-4 rounded">
                        <input type="email" placeholder="Email" class="text-white text-xl text-center focus:bg-blue-700 font-medium block  w-full bg-blue-800 px-4 mb-4 py-4 rounded">
                        <input type="password" placeholder="Set your Password" class="text-white text-xl text-center focus:bg-blue-700 font-medium block  w-full bg-blue-800 mb-4 px-4 py-4 rounded">
                        <input placeholder="Card Number" class="text-white text-xl text-center mb-4 focus:bg-blue-700 font-medium block  w-full bg-blue-800 px-4 py-4 rounded">
                        <button class="block w-full bg-yellow-600 px-4 py-4 mb-4 rounded uppercase font-bold text-yellow-900">Create my account</button>
                        <p class="text-white text-center text-sm font-semibold">Includes a 14 days trial before billing begins</p>
                    </form>
                </div>
              </div>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
import PlanSelector from './components/PlanSelector'

export default {
  name: 'App',
  components: {
      PlanSelector,
  }
}
</script>
