 <template>
    <div class="youtube-container">
      <iframe
        :src="embedUrl"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </template>
  
  <script>
  export default {
    name: "YouTubePlayer",
    props: {
      videoId: {
        type: String,
        required: true,
      },
    },
    computed: {
      embedUrl() {
        return `https://www.youtube.com/embed/${this.videoId}`;
      },
    },
  };
  </script>
  
  <style scoped>
  .youtube-container {
    display: flex;
    justify-content: center;
    margin: 20px 0;
  }
  
  iframe {
    width: 100%;
    max-width: 800px;
    height: 450px;
    border: none;
    border-radius: 8px;
  }
  </style>