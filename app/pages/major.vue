<script setup lang="ts">

const page = {
  "title":"Majors"
}

const posts = [
  {
      "title": 'EDUCATION',
      "description": "The Education program at Holy Family College is committed to developing compassionate, knowledgeable, and innovative educators who are prepared to make a positive impact in diverse educational settings. Our program emphasizes a holistic approach to teaching and learning, combining rigorous academic coursework with practical, real-world experience.",
      "image": {
        "src": "/Education.png"
      }
  }, {
      "title": 'NURSING',
      "description": "The Nursing program at Holy Family College is dedicated to preparing compassionate and skilled nursing professionals who are ready to meet the healthcare needs of diverse populations. Our program combines rigorous academic coursework with hands-on clinical experience, ensuring that our graduates are well-equipped to excel in the dynamic and rapidly evolving field of healthcare.",
      "image": {
        "src": "/Nursing.jpg"
      }
  }, {
      "title": 'Engineer',
      "description": "Welcome to the Theater Program at Holy Family College, where creativity, passion, and talent come together to create transformative theatrical experiences. Our program is designed to provide students with a comprehensive education in the performing arts, combining rigorous academic coursework with extensive hands-on experience.",
      "image": {
        "src": "/Engineer.png"
      }
  },{
      "title": 'LAW',
      "description": "Welcome to the Law Program at Holy Family College, where we are dedicated to cultivating the next generation of legal professionals who are committed to justice, integrity, and service. Our comprehensive and rigorous curriculum is designed to provide students with a deep understanding of the law, critical thinking skills, and practical experience necessary to excel in the legal field.",
      "image": {
        "src": "/Law.jpg",
      }
  }, {
      "title": 'PSYCHOLOGY',
      "description": "The Psychology program at Holy Family College offers a comprehensive and dynamic curriculum designed to provide students with a deep understanding of human behavior, mental processes, and psychological principles. Our program is dedicated to fostering intellectual curiosity, critical thinking, and a passion for helping others, preparing students for a wide range of careers and advanced studies in psychology and related fields.",
      "image": {
        "src": "/Psychology.png",
      }
  },{
      "title": 'COMMUNICATION',
      "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
      "image": {
        "src": "/Communication.png",
      }
  }
]

</script>

<template>
  <img class="imageplaceholder" src="/Library_i.png" >
  <UContainer>
    <UPageBody>
      <p class="college-info">
        Holy Family College has several colleges covering more than 60 fields of study with a full range of Bachelor's, Master's and Doctoral degree programmes for students.

        For example, the College of Business and Management, the College of Education and Leadership, the College of Arts and Sciences, and the College of Nursing and Health Sciences, etc.
      </p>
      <UBlogList>
        <UBlogPost
          v-for="(post, index) in posts"
          :key="index"
          :title="post.title"
          :description="post.description"
          :image="post.image"
          :ui="{description: 'line-clamp-2',image: {
    wrapper: 'ring-1 ring-gray-200 dark:ring-gray-800 relative overflow-hidden aspect-[3/4] w-full rounded-lg pointer-events-none',
    base: 'object-cover object-top w-full h-full transform transition-transform duration-200 group-hover:scale-105'
  },}"
        />
      </UBlogList>
    </UPageBody>
  </UContainer>
</template>

<style>
.college-info {
  font-family: 'Arial', sans-serif;
  font-size: 16px;
  line-height: 1.6;
  color: #333;
  max-width: 1300px;
  margin: 20px auto;
  padding: 20px;
  background-color: #f9f9f9;
  border-left: 4px solid #4a90e2;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: justify;
  transition: all 0.3s ease;
}

.college-info:hover {
  background-color: #fff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
  transform: translateY(-2px);
}

@media (max-width: 600px) {
  .college-info {
    font-size: 14px;
    padding: 15px;
    margin: 15px;
  }
}
</style>
