<template>
  <div class="about">
    <h2 id="about-header">About Us</h2>
    <p id="about-desc">At Jason's Drone Services, we capture breathtaking perspectives that elevate the way you see the
      world.
      Specializing in high-quality drone photography and videography, we bring a unique view to real estate, events,
      landscapes, and commercial projects. Our team combines technical expertise with a passion for storytelling to
      produce stunning aerial visuals that engage and inspire. Safety, precision, and creativity are at the heart of
      what we do. Whether you’re looking to showcase a property, document a special occasion, or simply explore new
      vantage points, our team is committed to delivering exceptional results that exceed expectations.</p>
    <img :src="require('@/assets/dronedelivery.png')" alt="dronedelivery" />
  </div>
  <div class="proj-1">
    <h2 id="projects-header">Projects</h2>
    <img :src="require('@/assets/droneconst.png')" alt="droneconst" />
    <h3>Construction Progress: City Skyline Apartments</h3>
    <p>Project Overview: Working with a large development firm, we documented the progress of their City Skyline
      Apartments project over the course of 18 months. Our team conducted monthly aerial shoots to provide clear,
      high-resolution footage of each construction phase. The video series enabled the client to showcase the
      construction process to investors, stakeholders, and the community, giving them valuable updates and a bird’s-eye
      view of the site’s transformation.</p>
    <p>Services Provided: Monthly aerial photography, progress documentation, time-lapse videography.</p>
    <p>Outcome: Improved stakeholder communication and project transparency, plus a final time-lapse video showing the
      entire build process.</p>
  </div>
  <div class="proj-2">
    <img :src="require('@/assets/dronefarm.png')" alt="dronefarm" />
    <h3>Agricultural Survey: Golden Harvest Vineyards</h3>
    <p>Project Overview: Working with Golden Harvest Vineyards, we performed aerial surveys to assess crop health,
      irrigation patterns, and potential pest issues across their vineyard. Using drones equipped with specialized
      cameras, we provided detailed images and data analysis for optimized farm management. This project allowed the
      client to increase yield efficiency, adjust water use, and reduce costs by targeting specific areas needing
      attention.</p>
    <p>Services Provided: Agricultural drone mapping, crop health analysis, NDVI imaging.</p>
    <p>Outcome: Optimized farm operations and targeted interventions, helping the client achieve a more sustainable and
      profitable harvest.</p>
  </div>
</template>

<style scoped>

.about {
  display: flex;
  flex-direction: column;
  margin: 15px 0px 5px 0px;
  padding: 5px 300px;
  background-color: #3C896D;
  border-radius: 5px;
  text-align: left;
  justify-content: start;

}

#about-header {
  width: 10%;
  height: auto;
  display: flex;
  text-align: center;
  padding-left: 10px;
  padding-right: 10px;
  color: #EDF2F4;
  background-color: #2c3e50;
}

#about-desc {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px;
  font-size: large;
  font-weight: bold;
}

#projects-header {
  width: 10%;
  max-height: auto;
  text-align: center;
  margin: 5px 2px;
  color: #EDF2F4;
  background-color: #2c3e50;
}

h3 {
  margin-left: 20px;
  text-decoration: underline;
  text-align: center;
}

.home p {
  display: flex;
  width: auto;
  text-align: left;
  margin: 20px;
  background-size: cover;
  margin-top: 5px;
  
}

.proj-1 {
  display: flex;
  flex-direction: column;
  margin: auto;
  padding: 20px 300px;
  max-width: max-content;
  max-height: max-content;
  background-color: #4D685A;
  border-radius: 5px;
  text-align: left;
  color: #EDF2F4;
  justify-content: start;
}

.proj-2 {
  display: flex;
  flex-direction: column;
  margin: auto;
  padding: 20px 300px;
  width: 50vmax;
  height: 50vmax;
  background-color: #546D64;
  margin-bottom: -20px;
  padding: 20px 300px;
  color: #EDF2F4;
  border-radius: 5px;
  text-align: left;
  color: #EDF2F4;
  justify-content: start;
}

.proj-1 img,
.proj-2 img,
.about img {
  display: flex;
  margin: auto;
  justify-content: center;
  align-items: center;
  max-width: 30vmax;
}
</style>