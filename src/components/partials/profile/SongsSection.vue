<template>
  <div>
    <div class="mx-auto py-4">
        <div class="flex flex-wrap font-bold text-gray-100">

          <div class="text-gray-900 text xl">Өлеңдер</div>
          <div class="bg-green-500 w-full h-1"></div>

          <div class="w-full mt-4">
            <RouterLinkButton
                btnText="Музыканы кетіру"
                class="ml-2"
                color="red"
                url="/account/delete-song"
            />
            <RouterLinkButton
                btnText="Музыка қосу"
                color="green"
                url="/account/add-song"
            />
          </div>
        </div>
    </div>


    <div class="pb-4">
      <SongPlayer />
      <YoutubeVideoSection/>
    </div>

  </div>
</template>


<script setup>

import RouterLinkButton from "@/components/global/RouterLinkButton";
import SongPlayer from "@/components/partials/profile/SongPlayer";
import YoutubeVideoSection from "@/components/partials/profile/YoutubeVideoSection";

</script>