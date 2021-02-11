<template>
  <div class="flex my-4 mx-8 items-center justify-between">
    <img src="profil.png" class="w-16 rounded-full hidden sm:block">
    <div>
      <NuxtLink v-for="link of links" :key="link.name" class="rounded-full p-4 pointer hover:bg-green-500 hover:text-white" :to="link.path">
        {{ link.name }}
      </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      links: [
        {
          name: 'Home',
          path: '/'
        },
        {
          name: 'Portfolio',
          path: '/portfolio'
        },
        {
          name: 'Contact',
          path: '/contact'
        }
      ]
    }
  }
}
</script>
