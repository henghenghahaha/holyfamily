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
      "title": "Library",
      "description": "The Holyfamily College Library is a vibrant hub of knowledge and learning. With its extensive collection of books, digital resources, and quiet study spaces, it caters to diverse academic needs. The library offers modern technology, expert librarians, and collaborative areas, fostering an environment of intellectual growth and research excellence. It stands as a cornerstone of the college's commitment to academic success and lifelong learning.",
      "id": "features",
      "img": "/Library.png",
      "align": "left"
    },
    {
      "title": "Music Center",
      "description": "The Music Center at Holyfamily College is a vibrant hub of artistic expression and musical education. Featuring state-of-the-art practice rooms, performance halls, and recording studios, it nurtures talent across various genres. With dedicated faculty and diverse programs, students explore composition, performance, and music technology. The center hosts regular concerts, workshops, and collaborations, fostering a dynamic community of musicians and music lovers.",
      "align": "right",
      "img": "music_centre.png"
    },
    {
      "title": "Student Dormitories",
      "description": "Holy Family College's Student Dormitories offer a welcoming home away from home for our diverse student body. These modern residences blend comfort with community, featuring well-equipped rooms, study areas, and common spaces that foster friendship and academic growth. With 24/7 security, on-site amenities, and a supportive residential life program, our dorms provide the ideal environment for students to thrive both personally and academically.",
      "align": "left",
      "img": "/student_dormitories.png"
    },
    {
      "title": "Dining Hall",
      "description": "Holy Family College's Dining Hall is a vibrant hub of community and culinary delight. This spacious, modern facility offers a diverse array of fresh, nutritious meals catering to various dietary needs. With its warm ambiance, students and faculty gather to enjoy delicious food, engage in lively conversations, and forge lasting friendships. The hall's commitment to sustainability and locally-sourced ingredients reflects the college's values of responsible stewardship.",
      "align": "right",
      "img": "/dining.png"
    }
  ]
}
</script>

<template>
  <div v-if="page">
    <img class="imageplaceholder" src="/campus_placeholder.jpg" />
    <div class="container2">
      <div class="stat-item">
        <div class="stat-number">3000+</div>
        <div class="stat-label">Global Students</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">100+</div>
        <div class="stat-label">Professional Course</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">1976</div>
        <div class="stat-label">Establishment Time</div>
      </div>
      <div class="stat-item">
        <div class="stat-number">500+</div>
        <div class="stat-label">Teachers</div>
      </div>
    </div>
    <ULandingSection
      v-for="(section, index) in page.sections"
      :key="index"
      :title="section.title"
      :description="section.description"
      :align="section.align"
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
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
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

