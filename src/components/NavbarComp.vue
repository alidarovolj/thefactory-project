<template>
  <div class="bg-black">
    <div class="container mx-auto">
      <div class="flex items-center justify-between py-9">
        <router-link to="/">
          <img src="../assets/img/logo.png" alt=""
        /></router-link>
        <router-link class="text-white flex items-center" to="/">
          <i class="fa-regular fa-heart mr-2.5 text-2xl"></i>
          <p class="text-lg">Избранное</p>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavbarComp",
};
</script>
