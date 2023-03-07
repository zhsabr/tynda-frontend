<template>
  <div class="container max-w-4xl mx-auto flex">
    <div class="w-1/3">
      <img class="w-full rounded-lg h-auto shadow-lg"
           src="https://via.placeholder.com/500"
           alt="Сурет">
    </div>
    <div class="w-full pl-4">
      <div class="flex">
        <div class="w-1/2">
          <h1 class="text-2xl md:text-4xl text-left text-gray-900">
            Сабыржан Жұмағалиев
          </h1>
          <span class="flex text-md text-gray-700 text-left">
              <i><b>Алматы, Казахстан</b></i>
          </span>
        </div>
        <div class="w-1/2 mt-2">
          <RouterLinkButton
            btnText="Профильді өңдеу"
            color="green"
            url="/account/edit-profile"
          />
        </div>
      </div>
      <ProfileIntoSection />
      <ProfileAboutSection />
    </div>
  </div>
  <SongSection/>
</template>

<script setup>

import ProfileIntoSection from "@/components/partials/profile/ProfileInfoSection";
import ProfileAboutSection from "@/components/partials/profile/ProfileAboutSection";
import SongSection from "@/components/partials/profile/SongsSection";
import RouterLinkButton from "@/components/global/RouterLinkButton";
</script>