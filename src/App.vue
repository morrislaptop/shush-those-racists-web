<template>
  <div id="app" class="p-8">
    <div class="flex justify-between">
      <div class="flex">
        <a href="#" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center mr-5"><i class="fab fa-twitter"></i></a>
        <a href="#" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center mr-5"><i class="fab fa-facebook-f"></i></a>
        <a href="#" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center"><i class="far fa-envelope"></i></a>
      </div>

      <a href="#" class="uppercase text-white border-2 border-red-orange p-4 tracking-wide font-black">Donate to the Goodies</a>
    </div>

    <div class="text-center max-w-md mx-auto">
      <p class="mb-4"><img alt="Shush Those Racists" src="./assets/shush.png"></p>
      <p class="mb-4 font-lato text-center tracking-wide font-bold text-white">Tired of racist Pollies like Bob Katter, Fraser Anning and Pauline Hanson making noise and filling up your feed?  Now you can shush those racists!</p>
      <p class="mb-8 font-lato text-center tracking-wide font-bold text-white">Shush Those Racists is a browser extension that replaces the names of our racist Politicians with colourful one liners, created by regular, non-racist Australians like you.</p>
      <p class="mb-8 text-2xl font-heavy text-white">Let’s call Bob Katter “that drunk racist uncle who hates Chinese people but eats the Chinese leftovers you were saving in the fridge”</p>
      <a href="#" class="inline-block uppercase text-red-orange p-4 tracking-wide font-black bg-white">Install in Chrome</a>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>

</style>
