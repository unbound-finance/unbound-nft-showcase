<template>
  <section class="h-auto  w-screen bg-gray-100 flex flex-col items-center justify-center">
    <div class="w-5/6 md:py-24 py-10 flex flex-col items-center justify-center">
      <div>
        <span
          class="md:text-6xl text-5xl font-bold bg-gradient-to-r from-green-400 to-blue-500 border-b-4 text-transparent bg-clip-text">Unbound's
          Exclusive NFTs</span>
      </div>
      <div class="grid grid-flow-row grid-cols-1 md:grid-cols-3 grid-rows-4 gap-12 md:pt-24 pt-10">
        <div v-for="(nftImage, id) in nftImages" :key="id">
          <span
            class="bg-white w-full h-full flex items-center justify-center bg-white p-5 rounded-2xl shadow-xl transition duration-500 ease-in-out hover:bg-gray-100 transform hover:-translate-y-2 hover:scale-60">
            <img class="rounded-2xl" :src="nftImage.image" alt="">
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        nftImages: [{
            id: 1,
            image: require("../assets/img/1.jpg"),
          },
          {
            id: 2,
            image: require("../assets/img/2.jpg"),
          },
          {
            id: 4,
            image: require("../assets/img/4.jpg"),
          },
          {
            id: 5,
            image: require("../assets/img/5.jpg"),
          },
          {
            id: 6,
            image: require("../assets/img/6.jpg"),
          },
          {
            id: 7,
            image: require("../assets/img/7.jpg"),
          },
          {
            id: 8,
            image: require("../assets/img/8.jpg"),
          },
          {
            id: 9,
            image: require("../assets/img/9.jpg"),
          },
          {
            id: 10,
            image: require("../assets/img/10.jpg"),
          },
          {
            id: 3,
            image: require("../assets/img/3.jpg"),
          },
        ]
      }
    }

  }

</script>

<style>

</style>
