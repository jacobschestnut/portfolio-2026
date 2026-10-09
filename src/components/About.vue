<template>
  <div class="main fade-in w-8/12 flex flex-col items-center lg:mb-64">

    <div class="bg-[#2f6661] rounded-3xl shadow-lg flex flex-col justify-center items-center lg:py-14 lg:px-24">
      <div class="border-2 border-[#ffaf87] rounded-xl px-6 py-2 w-fit mx-auto mt-5 mb-12">
        <h2 class="text-3xl lg:text-4xl font-semibold text-center">
          About
        </h2>
      </div>
      <div class="flex flex-col lg:flex-row justify-center items-center">

        <div class="text-container flex flex-col lg:mr-10">
          <p class="max-w-xl mb-5 text-base lg:text-lg font-semibold">
            I've been dabbling in Web Development, building gaming PCs and
            modifying/creating video games since 2011. It wasn't until I
            graduated with a completely separate degree in
            <a href="https://www.mtsu.edu/programs/audio-production/">
              Audio Engineering
            </a>
            that I considered making a career out of Software Development.
          </p>

          <p class="max-w-xl mb-5 text-base lg:text-lg font-semibold">
            Since graduating from
            <a href="https://nashvillesoftwareschool.com/">
              Nashville Software School
            </a>
            in 2022, I began my professional journey as an Application
            Developer at a major insurance company while also diving into iOS
            Development and other personal projects. I'm always looking for opportunities
            to expand my skillset even more.
          </p>
        </div>

        <div class="hidden lg:block overflow-hidden h-80">
          <img class="object-cover w-full h-full rounded-xl" src="/assets/images/portrait.jpg" alt="profile-picture" />
        </div>

      </div>
    </div>
  </div>
</template>

<script setup>
import useFadeIn from "../composables/fadein";

useFadeIn();
</script>

<style scoped>
a {
  color: #ffaf87;
  text-decoration: underline;
}

a:hover {
  text-decoration: none;
}
</style>