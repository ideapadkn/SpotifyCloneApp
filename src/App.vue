<script setup>
import { ref } from 'vue';
import { RouterLink, RouterView } from 'vue-router';

import ChevronUp from 'vue-material-design-icons/ChevronUp.vue';
import ChevronDown from 'vue-material-design-icons/ChevronDown.vue';
import ChevronRight from 'vue-material-design-icons/ChevronRight.vue';
import ChevronLeft from 'vue-material-design-icons/ChevronLeft.vue';

let openMenu = ref(false)
</script>

<template>
  <div>
    <div 
      class="
        w-[calc(100%-240px)]
        h-[60px]
        fixed
        right-0
        z-20
        bg-[#101010]
        bg-opacity-80
        flex
        items-center
        justify-between
      "
    >  
      <div class="flex items-center ml-6">
        <button type="button" class="rounded-full bg-black p-[1px] cursor-pointer">
          <ChevronLeft fillColor="#ffffff" :size="30" />
        </button>
        <button type="button" class="rounded-full bg-black p-[1px] ml-4 cursor-pointer">
          <ChevronRight fillColor="#ffffff" :size="30" />
        </button>
      </div>

      <button 
        @click="openMenu = !openMenu" :class="openMenu ? 'bg-[#282828]' : 'bg-black'"
        class="bg-black hover:bg-[#282828] rounded-full p-0.5 mr-8 mt-0.5 cursor-pointer"
      >
        <div class="flex items-center">
          <img
            class="rounded-full"
            width="27"
            src="https://yt3.ggpht.com/mNayJUx6ovSmnBOt_o2oRY6IhyyKQAATb6tn5FzjJeVr0Em-4LajvYFLuUmR6fOzuaYrv9I1GA=s88-c-k-c0x00ffffff-no-rj"
          >
          <div class="text-white text-[14px] ml-1.5 font-semibold">Ideapad</div>
          <ChevronDown v-if="!openMenu" @click="openMenu = true" fillColor="#ffffff" :size="25" />
          <ChevronUp v-else @click="openMenu = false" fillColor="#ffffff" :size="25" />
        </div>
      </button>

      <span
        v-if="openMenu"
        class="fixed w-[190px] bg-[#282828] shadow-2xl z-50 rounded-sm top-[52px] right-[35px] p-1 cursor-pointer"
      >
      <ul class="text-gray-200 font-semibold text-[14px]">
        <li class="px-3 py-2.5 hover:bg-[#3e3d3d] border-b border-b-gray-600">Profile</li>
        <li class="px-3 py-2.5 hover:bg-[#3e3d3d]">Log out</li>
      </ul>
      </span>
    </div>

    <div
      id="sideNow"
      class="h-[100%] p-6 w-[240px] fixed z-50 bg-black"
    >

    </div>

  </div> 
</template>

