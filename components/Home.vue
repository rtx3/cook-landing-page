<template>
  <main class="py-16 flex gap-16 flex-col <lg:py-4">
    <section class="flex justify-between gap-32 <lg:(flex-col p-4 gap-16)">
      <div class="flex-1 flex flex-col gap-6 relative">
        <h1 class="text-48px line-height-1em font-bold title">
          {{ SiteDescription }}
        </h1>
        <p class="text-hint">{{ SiteIntro }}</p>
        <div class="flex items-center justify-between">
          <div class="flex items-center">
            <!--
            <div v-for="user in UserList" :key="user" class="-mr-2.5">
              <img class="rounded-1/2 w-8 h-8" :src="user" alt="" />
            </div>
            -->
            <div class="ml-8 whitespace-nowrap">
              Used by <a class="text-primary">1000+</a> enthusiasts
            </div>
          </div>
        </div>
        <!--
        <button
          class="bg-primary text-white w-fit flex gap-2 px-4 py-3 rounded-4 cursor-pointer"
        >
        We are live and you’re officially invited to see what’s new. Download on the App Store today. 
          <div class="i-ion-arrow-right-c"></div>
        </button>
        -->
        <a
          href="https://apps.apple.com/us/app/%E5%BF%AB%E9%80%89%E7%83%B9%E9%A5%AA/id6474119619?itsct=apps_box_link&itscg=30200"
          target="_blank"
          class="w-fit"
          ><img
            src="/QuickCook-CN-B.png"
            alt="https://apple.co/3HtjF6M"
            style="width: 500px; height: 280px"
            width="250"
            height="54"
        /></a>
        <div class="absolute top-1/4 opacity-25 background">
          <div class="bg-primary w-40 h-20 blur-50 top-5 left-0 absolute"></div>
          <div
            class="bg-danger w-40 h-20 blur-50 top-60 left-40 absolute"
          ></div>
          <div
            class="bg-success w-40 h-20 blur-50 top-30 left-20 absolute"
          ></div>
        </div>
      </div>
      <div class="flex-1">
        <TiltCard></TiltCard>
      </div>
    </section>
    <!--
    <Example></Example>
    <Comment></Comment>
    <Price></Price>
    <FAQ></FAQ>
    -->
     <!--
    <section class="w-full center flex-col gap-8">
      <h2 class="text-24px font-bold line-height-1em">
        Unlock your first card
      </h2>
      <button
        class="bg-primary text-white w-fit flex gap-2 px-8 py-3 rounded-4 cursor-pointer"
      >
        Get Started
      </button>
    </section>
    -->
    <AutoUp></AutoUp>
  </main>
</template>

<script setup lang="ts">
  import { SiteDescription, SiteIntro } from '~/config'
  const UserList = [
    '/images/j.jpg',
    '/images/d.jpg',
    '/images/k.jpg',
    '/images/l.jpg',
    '/images/d.avif',
    '/images/m.jpg',
  ]
</script>

<style lang="scss" scoped>
  .title {
    background: linear-gradient(
      to right,
      rgb(var(--color-danger)) 20%,
      rgb(var(--color-primary))
    );
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  @keyframes background {
    0% {
      transform: translate(0, 0) rotate(0deg);
    }

    50% {
      transform: translate(50px, -50px) rotate(1turn);
    }

    100% {
      transform: translate(-50px, 50px) rotate(0deg);
    }
  }
</style>
