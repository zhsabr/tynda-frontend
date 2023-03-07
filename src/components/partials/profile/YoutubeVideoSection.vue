<template>
  <div>
    <div class="mx-auto py-4">
        <div class="flex flex-wrap font-bold text-gray-100">

          <div class="text-gray-900 text xl">Youtube видеолар</div>
          <div class="bg-green-500 w-full h-1"></div>

          <div class="w-full mt-4">
            <RouterLinkButton
                btnText="Видеоны кетіру"
                class="ml-2"
                color="red"
                url="/account/delete-youtube-video"
            />
            <RouterLinkButton
                btnText="Видео қосу"
                color="green"
                url="/account/add-youtube-video"
            />
          </div>
        </div>
    </div>


    <div class="flex flex-wrap mb-4 ">

      <div class="my-1 px-1 w-full md:w-1/2 lg:w-1/2">
        <div class="text-xl text-gray-900">Видеоның аты</div>
        <iframe class="w-full h-60 mt-2" src="https://www.youtube.com/embed/_wwcwQxnLVI?autoplay=0" frameborder="0"></iframe>
      </div>

    </div>

  </div>
</template>


<script setup>

import RouterLinkButton from "@/components/global/RouterLinkButton";
</script>