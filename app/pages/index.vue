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
<!--    <ULandingHero-->
<!--      :ui="{title: 'text-3xl font-serif font-semibold tracking-tight text-gray-900 dark:text-white sm:text-7xl'}"-->
<!--    >-->

<!--    </ULandingHero>-->
    <img class="imageplaceholder" src="/campus_placeholder.jpg" />
<!--    <ULandingSection class="!pt-0">-->
<!--      <ImagePlaceholder/>-->
<!--    </ULandingSection>-->

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

<!--    <ULandingSection>-->
<!--      <div class="container1">-->
<!--        <img class="image1" src="/Class.jpg" alt="Holy Family College">-->
<!--      </div>-->
<!--    </ULandingSection>-->
  </div>
</template>

<style scoped>
.landing-grid {
  background-size: 100px 100px;
  background-image: linear-gradient(to right, rgb(var(--color-gray-200)) 1px, transparent 1px),
  linear-gradient(to bottom, rgb(var(--color-gray-200)) 1px, transparent 1px);
}

.dark {
  .landing-grid {
    background-image: linear-gradient(to right, rgb(var(--color-gray-800)) 1px, transparent 1px),
    linear-gradient(to bottom, rgb(var(--color-gray-800)) 1px, transparent 1px);
  }
}

.imageplaceholder {
  width: 1920px;
  //height: 80%;
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

.container1 {
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  text-align: center;
  max-width: 1200px;
  position: relative;
}

.image1 {
  width: 100%;
  margin-bottom: 20px;
  border-radius: 10px;
}
</style>

