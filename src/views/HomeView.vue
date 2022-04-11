<template>
  <div>
    <navbar />
    <div class="home">
      <div class="set_search">
        <form action="">
          <div class="container mx-auto py-24 relative w-1/2">
            <input
              class="block mx-auto px-10 py-5 text-black w-full"
              type="text"
              placeholder="Поиск"
            />
            <i
              class="fa fa-magnifying-glass set_button hover:cursor-pointer"
            ></i>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import navbar from "../components/NavbarComp.vue"
export default {
  name: "HomeView",
  components: {
    navbar
  },
  data() {
    return {
      accessKey: "UxQcyiv7djwaIznmB6G73bYjldVCcICcUT4HZpscGcI",
      url: "https://api.unsplash.com/",
      photos: null,
    };
  },
  async mounted() {
    const res = await axios.get(
      this.url + "?client_id=${" + this.accessKey + "}"
    );
    console.log(res);
    this.photos = res.data;
  },
};
</script>
