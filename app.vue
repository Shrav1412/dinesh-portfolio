<template>
  <div>
    <div class="pt-20 pl-20 h-screen bg-[#cfc8c3] grid grid-cols-3 pb-24">
      <div class="col-span-2">
        <div class="flex justify-around">
          <div>
            <h1 class="font-semibold text-3xl">Dinesh T E<sup>®</sup></h1>
          </div>
          <div>
            <p class="w-[350px] text-justify">
              Welcome to the world as seen through the lens of Dinesh Elango, an acclaimed photographer specializing in
              both nature and people, Kōsuke possesses an innate ability to encapsulate the essence of life's beautiful
              moments in his images.
            </p>
          </div>
        </div>
        <div class="mt-44">
          <h1 class="ml-20 font-bold text-9xl">DINESH T E<sup>®</sup></h1>
          <button @click="scrollToPhotography()"
            class="mt-10 ml-20 rounded-3xl w-[150px] h-[50px] bg-[#1d1b19] text-[#cfc8c3]">View portfolio</button>
        </div>
        <div class="mt-40 ">
          <div class="flex justify-between px-44">
            <h1 class="text-[#1d1b19]">From Chennai, India</h1>
            <p class="w-[450px] text-justify">This online portfolio is an exploration into Kōsuke's unique photographic
              perspective. A journey into the
              spaces we inhabit, the people we encounter, and the collective stories we share. We invite you to browse
              through the collection, feel the passion behind each photograph, and embark on a visual journey like no
              other.
            </p>
          </div>
        </div>
      </div>
      <div>
        <img class="hover:scale-105 duration-1000 mt-20 rounded-3xl w-[500px]" src="./assets/dinesh.jpg" alt="dinesh" />
      </div>
    </div>
    <div ref="photography" id="photography" class=" pt-20 h-screen pb-20 bg-[#1d1b19]">
      <h1 class="text-[#cfc8c3] pl-10 font-semibold text-4xl">Dinesh's Photography
      </h1>
      <div class="grid grid-cols-3 place-items-center mt-32">
        <div>
          <h1 class="text-sm text-[#cfc8c3]">MAY 2022 | CHENNAI, INDIA</h1><br>
          <h1 class="text-2xl font-semibold text-[#cfc8c3]">Portraits of Dinesh</h1><br>
          <p class="text-[#cfc8c3] w-[400px] text-justify">Enter the bustling world of beaches through Dinesh's lens as
            he captures the captivating essence of people navigating the vibrant cityscape. In this series, Dinesh
            delves into the unique rhythm and energy found within the heart of beaches.
          </p><br><br><br>
          <img class="hover:scale-105 duration-1000 rounded-3xl w-[400px]" src="./assets/d3.png" alt="dinesh" />
        </div>
        <div>
          <img class="hover:scale-105 duration-1000 w-[395px] rounded-3xl" src="./assets/d2.png" alt="dinesh" />
        </div>
        <div>
          <img class="hover:scale-105 duration-1000 w-[450px] rounded-3xl" src="./assets/d1.png" alt="dinesh" />
        </div>
      </div>
      <div class="bg-[#1d1b19] h-screen pt-20 px-32">
        <div class="grid grid-cols-3 justify-self-stretch">
          <div class=" col-span-2">
            <img class="hover:scale-105 duration-1000 rounded-3xl justify-start w-[1000px] h-[400px]"
              src="./assets/1.jpg" alt="scene">
          </div>
          <div class="items-end flex flex-col justify-center">
            <h1 class="text-sm text-[#cfc8c3]">NOVEMBER 2023 | SIKKIM, INDIA</h1><br>
            <h1 class="text-2xl font-semibold text-[#cfc8c3]">A Symphony of Sikkim Wonders</h1><br>
            <p class="text-[#cfc8c3] w-[400px] text-justify">Step into the mesmerizing world of Dinesh's nature
              series, where the beauty of the natural world unfolds in breathtaking detail. Through his lens, Dinesh
              captures the harmony and grandeur of Earth's landscapes, from vast mountain ranges to delicate beach
              waves.
            </p>
          </div>
        </div>
        <div class="grid grid-cols-3 gap-16 place-items-center pt-20">
          <div><img class="hover:scale-105 duration-1000 w-[500px] rounded-3xl" src="./assets/2.jpg" alt="img"></div>
          <div><img class="hover:scale-105 duration-1000 w-[500px] rounded-3xl" src="./assets/3.jpg" alt="img"></div>
          <div><img class="hover:scale-105 duration-1000 w-[500px] rounded-3xl" src="./assets/4.jpg" alt="img"></div>
        </div>
      </div>
      <div class="bg-[#1d1b19] h-screen pt-20 px-32">
        <div class="grid grid-cols-3 place-items-center">
          <div class="text-[#cfc8c3]">
            <h1 class="text-sm">FEBRUARY 2024 | GANGTOK, INDIA</h1><br>
            <h1 class="text-2xl font-semibold">Bright Clicks : Mountains & Rivers</h1><br>
            <p class="w-[400px] text-justify">
              Embark on a tranquil journey through the sacred temples and serene spaces of Kyoto, as Kōsuke Nakamura's
              lens unveils the profound beauty and spiritual essence of this ancient city. In this captivating series,
              Kōsuke captures the timeless tranquility and meditative atmosphere that permeate the temples of Kyoto.
            </p><br><br><br>
            <img class="hover:scale-105 duration-1000 w-[400px] rounded-3xl" src="./assets/6.jpg" alt="mount" />
          </div>
          <div class="col-span-2">
            <img class=" hover:scale-105 duration-1000 h-[600px] rounded-3xl" src="./assets/5.jpg" alt="river">
          </div>
        </div><br><br><br><br><br>
        <hr>
        <div class="text-[#cfc8c3] pt-16 text-lg font-medium flex justify-between items-center">
          <h1>Dinesh T E<sup>®</sup></h1>
          <h1>© 2024 Dinesh T E. All rights reserved.</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
html {
  scroll-behavior: smooth;
}
</style>

<script>
export default {
  methods: {
    scrollToPhotography() {
      this.$nextTick(() => {
        const photographySection = this.$refs.photography;
        photographySection.scrollIntoView({ behavior: 'smooth' });
      });
    }
  }
}
</script>
