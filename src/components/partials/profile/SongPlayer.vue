<template>
  <div class="bg-green-500 rounded">
    <div id="aplayer"></div>
  </div>
</template>


<script setup>
import {onMounted} from "vue";
import 'aplayer/dist/APlayer.min.css';
import APlayer from 'aplayer'

onMounted(() =>{
  thePlayer()
})

const thePlayer = () => {
  new APlayer({
    container: document.getElementById('aplayer'),
    audio: [
      {
        name: 'Бірінші',
        artist: 'artist',
        url: '/music/cinematic-time-lapse.mp3',
        cover: 'cover.jpg'
      },
      {
        name: 'Екінші',
        artist: 'artist',
        url: '/music/inspiring-emotional-uplifting-piano.mp3',
        cover: 'cover.jpg'
      },
    ]
  });
}
</script>