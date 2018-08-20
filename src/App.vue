<template>
  <div id="app" class="p-8">
    <div class="flex justify-between">
      <div class="flex">
        <a :href="twitterUrl" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center mr-5"><i class="fab fa-twitter"></i></a>
        <a :href="facebookUrl" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center mr-5"><i class="fab fa-facebook-f"></i></a>
        <a :href="emailUrl" class="border-2 border-red-orange rounded-full p-4 w-8 h-8 text-white center-center"><i class="far fa-envelope"></i></a>
      </div>

      <a :href="donateUrl" class="uppercase text-white border-2 border-red-orange p-4 tracking-wide font-black">Donate to the Goodies</a>
    </div>

    <div class="text-center max-w-md mx-auto">
      <p class="mb-4"><img alt="Shush Those Racists" src="./assets/shush.png"></p>
      <p class="mb-4 font-lato text-center tracking-wide font-bold text-white">Tired of racist pollies like Bob Katter, Fraser Anning and Pauline Hanson making noise and filling up your feed? Now you can shush those racists!</p>
      <p class="mb-8 font-lato text-center tracking-wide font-bold text-white">Shush Those Racists is a browser extension that replaces the names of our racist politicians with colourful one liners, created by regular, non-racist Australians like you.</p>
      <p class="mb-8 text-2xl font-heavy text-white">Got a witty line? We want to hear it. Submit <a class="text-white underline" href="https://shushthoseracists.typeform.com/to/Z4sjSJ">here</a>.</p>
      <p class="mb-8 text-2xl font-heavy text-white">#Shushthoseracists</p>
      <a :href="extUrl" class="inline-block uppercase text-red-orange p-4 tracking-wide font-black bg-white">Install in Chrome</a>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    facebookUrl () {
      return `https://www.facebook.com/sharer.php?u=${process.env.VUE_APP_SHARE_URL}` 
    },

    twitterUrl () {
      return `https://twitter.com/intent/tweet?text=Tired of racist pollies like Bob Katter, Fraser Anning and Pauline Hanson making noise and filling up your feed?&hashtags=Shushthoseracists&url=${process.env.VUE_APP_SHARE_URL}`
    },

    emailUrl () {
      return `mailto:?subject=It’s time to shush those racist Australian politicians&body=Tired of racist pollies like Bob Katter, Fraser Anning and Pauline Hanson making noise and filling up your feed? Shushthoseracists.org #Shushthoseracists`
    },

    extUrl () {
      return process.env.VUE_APP_EXT_URL
    },

    donateUrl () {
      return process.env.VUE_APP_DONATE_URL
    },
  }
}
</script>