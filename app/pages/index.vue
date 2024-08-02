<script setup lang="ts">

const page = {
  "title": "Holy Family College",
  "description": "",
  "navigation": "False",
  "hero": {
    "title": "Holy Family College"
  },
  "sections": [
    {
      "title": "Music Center",
      "description": "The Music Center at Holyfamily College is a vibrant hub of artistic expression and musical education. Featuring state-of-the-art practice rooms, performance halls, and recording studios, it nurtures talent across various genres. With dedicated faculty and diverse programs, students explore composition, performance, and music technology. The center hosts regular concerts, workshops, and collaborations, fostering a dynamic community of musicians and music lovers.",
      "align": "right",
      "img": "music_centre.png"
    },
    {
      "title": "Library",
      "description": "The Holyfamily College Library is a vibrant hub of knowledge and learning. With its extensive collection of books, digital resources, and quiet study spaces, it caters to diverse academic needs. The library offers modern technology, expert librarians, and collaborative areas, fostering an environment of intellectual growth and research excellence. It stands as a cornerstone of the college's commitment to academic success and lifelong learning.",
      "id": "features",
      "img": "/Library.png",
      "align": "left"
    },
    {
      "title": "Campus Life",
      "description": "Holy Family College offers a vibrant campus experience, blending academic excellence with a close-knit community. Students enjoy a range of activities, from clubs and sports to cultural events. The picturesque campus fosters personal growth and lifelong friendships. With modern facilities, cozy dorms, and a supportive atmosphere, students find a perfect balance between study and social life, creating unforgettable memories throughout their college journey.",
      "align": "right",
      "img": "/campuslife.png"
    }
  ]
}
</script>

<template>
  <div v-if="page">
    <img class="imageplaceholder" src="/campus_placeholder.jpg" />
    <div class="container2">
      <div class="stat-item">
        <div class="stat-number">1885</div>
        <div class="stat-label">Establishment</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">100+</div>
        <div class="stat-label">Academic programmes</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">300+</div>
        <div class="stat-label">Teachers</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">4000+</div>
        <div class="stat-label">Global Students</div>
      </div>
    </div>

    <div class="flex flex-wrap -mx-2">
      <div class="w-full sm:w-1/3 px-2 mb-4">
        <img
          src=""
          class="w-full h-auto rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300"
        />
      </div>
      <div class="w-full sm:w-1/3 px-2 mb-4">
        <img
          src=""
          class="w-full h-auto rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300"
        />
      </div>
      <div class="w-full sm:w-1/3 px-2 mb-4">
        <img
          src=""
          class="w-full h-auto rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300"
        />
      </div>
    </div>

    <ULandingSection
      v-for="(section, index) in page.sections"
      :key="index"
      :title="section.title"
      :description="section.description"
      :align="section.align"
      :ui="{wrapper: 'py-8 sm:py-8'}"
    >
      <div class="container">
        <img class="image" :src=section.img alt="Holy Family College">
      </div>
    </ULandingSection>

  </div>
</template>

<style scoped>

.imageplaceholder {
  width: 1920px;
}

.container {
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  max-width: 600px;
  position: relative;
}

.image {
  width: 100%;
  height: auto;
  margin-bottom: 20px;
  border-radius: 10px;
}

.container2 {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100%;
  max-width: 1900px;
  padding: 20px;
  height: 200px;
  background-color: rgb(20,50,150);
}

.stat-item {
  text-align: center;
  padding: 20px;
  color: #FFFFFF;
}

.stat-number {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 10px;
}

.stat-label {
  font-size: 1rem;
  opacity: 0.8;
}

@media (max-width: 768px) {
  .container2 {
    flex-direction: column;
  }
  .stat-item {
    margin-bottom: 30px;
  }
}

</style>

