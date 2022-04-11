<template>
  <div class="bg-black">
    <div class="container mx-auto">
      <div class="flex items-center justify-between py-6">
        <router-link to="/">
          <img class="h-11 w-auto" src="../assets/img/logo.png" alt=""
        /></router-link>
        <div class="flex items-center">
          <router-link class="text-white flex items-center" to="/">
            <i class="fa fa-magnifying-glass mr-2.5 text-2xl"></i>
            <p class="text-xl">Поиск</p>
          </router-link>
          <router-link class="text-white flex items-center ml-9" to="/">
            <i class="fa-regular fa-heart mr-2.5 text-2xl"></i>
            <p class="text-xl">Избранное</p>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavbarComp",
};
</script>
