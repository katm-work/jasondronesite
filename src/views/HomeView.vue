<template>
  <h2>About us</h2>
  <div id="about-content">
    <img id= "about-img":src="require('@/assets/droneairview.jpg')" alt="droneairview" />
    <p id="about-desc">At Jason's Drone Services, we capture breathtaking perspectives that elevate the way you see the
      world. Specializing in high-quality drone photography and videography, we bring a unique view to real estate, events,
      landscapes, and commercial projects. Our team combines technical expertise with a passion for storytelling to
      produce stunning aerial visuals that engage and inspire. Safety, precision, and creativity are at the heart of
      what we do. Whether you’re looking to showcase a property, document a special occasion, or simply explore new
      vantage points, our team is committed to delivering exceptional results that exceed expectations.</p>
  </div>
    <h2>Projects</h2>
  <div class="article-container">
    <ContentList :contents="articles" />
  </div>
</template>

<script>
import ContentList from "../components/Projects.vue";
import dronefarm from "../assets/dronefarm.png"
import droneconst from "../assets/droneconst.png"


export default {
  name: "App",
  components: {
    ContentList,
  },
  data() {
    return {
      articles: [
        {
          title: "Construction Progress: City Skyline Apartments",
          text1: "Working with a large development firm, we documented the progress of their City Skyline Apartments project over the course of 18 months. Our team conducted monthly aerial shoots to provide clear, high-resolution footage of each construction phase. The video series enabled the client to showcase the construction process to investors, stakeholders, and the community, giving them valuable updates and a bird’s-eye view of the site’s transformation.",
          text2: "Monthly aerial photography, progress documentation, time-lapse videography.",
          text3: "Improved stakeholder communication and project transparency, plus a final time-lapse video showing the entire build process.",
          image: droneconst,
          alt: "Drone used for construction surveying",
        },
        {
          title: "Agricultural Survey: Golden Harvest Vineyards",
          text1: "Working with Golden Harvest Vineyards, we performed aerial surveys to assess crop health, irrigation patterns, and potential pest issues across their vineyard. Using drones equipped with specialized cameras, we provided detailed images and data analysis for optimized farm management. This project allowed the client to increase yield efficiency, adjust water use, and reduce costs by targeting specific areas needing attention.",
          text2: "Agricultural drone mapping, crop health analysis, NDVI imaging.",
          text3: "Optimized farm operations and targeted interventions, helping the client achieve a more sustainable and profitable harvest.",
          image: dronefarm,
          alt: "Drone used to survey farmlands",
        },
      ],
    };
  },
};
</script>

<style scoped>

#about-img {
  display: flex;
  margin: auto;
  justify-content: center;
  align-items: center;
  width: 600px;
  border-radius: 4px ;
  border: solid #0A100DA3;
}

#about-desc{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width:40%;
  height: 100%;
  margin: 20px auto;
  overflow-wrap: break-word;
  text-shadow: 2px 2px #0A100DA3;
  font-size: larger;
  font-weight: bold;
}
  



.article-container {  
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width:40%;
  height: 100%;
  margin: auto;
  overflow-wrap: break-word;
  
}

</style>
