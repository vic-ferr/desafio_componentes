<template>
  <div id="app">
    <RickMorty v-for="(comic, i) in comics" :key="i" :animex="comic" />
  </div>
</template>

<script>
import RickMorty from "@/components/RickMorty";

export default {
  name: "App",
  components: {
    RickMorty,
  },
  data() {
    return {
      comics: [
        {
          name: "Rick Sanchez",
          image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          name: "Morty Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          name: "Summer Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },

        {
          name: "Beth Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          name: "Jerry Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
      ],

      bgImagen:
        "https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png",
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #05aa1b;
  margin-top: 60px;
  background-image: url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png);
  background-position: cover;
}
.imagen-rick {
  border-radius: 50%;
}

.box-rick-and-morty {
  display: flex;
  padding-top: 15px;
}
.box-name-h3 {
  padding: 35px;
  margin-left: 35px;
}
</style>
