
<template>
  <div id="video-container">
    <h2>Our Services</h2>
    
    <div class="button-group">
      <button class="styled-btn" @click="selectVideo('tN_Qm0Zxoz4')">Aerial Photography</button>
      <button class="styled-btn" @click="selectVideo('kwtJpmFVSWw')">Building Videography</button>
      <button class="styled-btn" @click="selectVideo('KturnnX5XWM')">Land Survey</button>
    </div>
    
    <YouTubePlayer v-if="currentVideo" :videoId="currentVideo" />
  </div>
</template>
<script>
import YouTubePlayer from "@/components/VideoPlayer.vue";

export default {
  name: "App",
  components: {
    YouTubePlayer,
  },
  data() {
    return {
      currentVideo: "tN_Qm0Zxoz4", 
    };
  },
  methods: {
    selectVideo(videoId) {
      this.currentVideo = videoId;
    },
  },
};
</script>

<style scoped>
h1 {
  text-align: center;
  margin-bottom: 20px;
}
</style>

<style scoped>

#video-container {
    height: 42em;
}
.styled-btn {
    background-color: #2c3e50;
    color: #EDF2F4;
    padding: 10px 20px;
    border-bottom: 3px solid #EDF2F4;
    border-right: 2px solid #EDF2F4;
    border-top: 1px solid #EDF2F4;
    border-left: 1px solid #EDF2F4;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
    text-shadow: 2px 2px #0A100DA3;
    transition: background-color 0.3s ease;
    background-color: #8AA8A1;
}

.styled-btn:hover{
    background-color: #2980b9;
}


.button-group {
    margin-bottom: 1em;
}

button {
    margin-right: 10px;
}

</style>