<script setup>
import HomeCard from '../components/HomeCard.vue';
</script>

<template>
  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl font-semibold hover:underline cursor-pointer"
    >
      Podcasts to make you smarter
    </button>

    <div class="py-1.5"></div>

    <div class="flex items-center">
      <HomeCard image="https://picsum.photos/id/30/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard image="https://picsum.photos/id/45/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="md:block hidden" image="https://picsum.photos/id/65/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="lg:block hidden" image="https://picsum.photos/id/67/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="xl:block hidden" image="https://picsum.photos/id/100/300/300" title="Title is here" subTitle="subTitle is here" />
    </div>
  </div>
  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl font-semibold hover:underline cursor-pointer"
    >
      Recommended Radio 
    </button>

    <div class="py-1.5"></div>

    <div class="flex items-center">
      <HomeCard image="https://picsum.photos/id/31/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard image="https://picsum.photos/id/46/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="md:block hidden" image="https://picsum.photos/id/62/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="lg:block hidden" image="https://picsum.photos/id/60/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="xl:block hidden" image="https://picsum.photos/id/110/300/300" title="Title is here" subTitle="subTitle is here" />
    </div>
  </div>
  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl font-semibold hover:underline cursor-pointer"
    >
      Recommended Songs
    </button>

    <div class="py-1.5"></div>

    <div class="flex items-center">
      <HomeCard image="https://picsum.photos/id/38/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard image="https://picsum.photos/id/49/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="md:block hidden" image="https://picsum.photos/id/75/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="lg:block hidden" image="https://picsum.photos/id/17/300/300" title="Title is here" subTitle="subTitle is here" />
      <HomeCard class="xl:block hidden" image="https://picsum.photos/id/103/300/300" title="Title is here" subTitle="subTitle is here" />
    </div>
  </div>
</template>
