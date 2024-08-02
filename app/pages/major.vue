<script setup lang="ts">

const page = {
  "title":"Majors"
}

const programs = [
  {"id":1,
      "title": 'EDUCATION',
      "description": "The Education program at Holy Family College is committed to developing compassionate, knowledgeable, and innovative educators who are prepared to make a positive impact in diverse educational settings. Our program emphasizes a holistic approach to teaching and learning, combining rigorous academic coursework with practical, real-world experience.",
      "image": {
        "src": "/Education.png"
      }
  }, {
    "id":2,
      "title": 'NURSING',
      "description": "The Nursing program at Holy Family College is dedicated to preparing compassionate and skilled nursing professionals who are ready to meet the healthcare needs of diverse populations. Our program combines rigorous academic coursework with hands-on clinical experience, ensuring that our graduates are well-equipped to excel in the dynamic and rapidly evolving field of healthcare.",
      "image": {
        "src": "/Nursing.jpg"
      }
  }, {"id":3,

      "title": 'Engineer',
      "description": "Welcome to the Theater Program at Holy Family College, where creativity, passion, and talent come together to create transformative theatrical experiences. Our program is designed to provide students with a comprehensive education in the performing arts, combining rigorous academic coursework with extensive hands-on experience.",
      "image": {
        "src": "/Engineer.png"
      }
  },{
    "id":4,
      "title": 'LAW',
      "description": "Welcome to the Law Program at Holy Family College, where we are dedicated to cultivating the next generation of legal professionals who are committed to justice, integrity, and service. Our comprehensive and rigorous curriculum is designed to provide students with a deep understanding of the law, critical thinking skills, and practical experience necessary to excel in the legal field.",
      "image": {
        "src": "/Law.jpg",
      }
  }, {
    "id":5,
      "title": 'PSYCHOLOGY',
      "description": "The Psychology program at Holy Family College offers a comprehensive and dynamic curriculum designed to provide students with a deep understanding of human behavior, mental processes, and psychological principles. Our program is dedicated to fostering intellectual curiosity, critical thinking, and a passion for helping others, preparing students for a wide range of careers and advanced studies in psychology and related fields.",
      "image": {
        "src": "/Psychology.png",
      }
  },{
    "id":6,
      "title": 'COMMUNICATION',
      "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
      "image": {
        "src": "/Communication.png",
      }
  },{
    "id":7,
    "title": 'ART',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/Art.png",
    }
  },{
    "id":8,
    "title": 'BUSSINESS',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/Business.png",
    }
  },{
    "id":9,
    "title": 'Foreign Languages',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/ForeignLanguages.jpg",
    }
  },{
    "id":10,
    "title": 'ECONOMICS',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/Economics.png",
    }
  },{
    "id":11,
    "title": 'HUMANITIES',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/Humanities.jpg",
    }
  },{
    "id":12,
    "title": 'Internation Relationship',
    "description": "The Communication program at Holy Family College is designed to equip students with the skills and knowledge necessary to excel in a rapidly evolving media landscape. Our program emphasizes both the theoretical foundations and practical applications of communication, preparing graduates for diverse careers in media, public relations, corporate communication, journalism, and more.",
    "image": {
      "src": "/InternationalRelations.jpg",
    }
  }
]

</script>

<template>
  <div class="image-container">
    <img class="imageplaceholder" src="/Library_i.png" alt="Library Image">
    <div class="text-overlay">
      <p class="college-description">
        Holy Family College has several colleges covering more than 60 fields of study with a full range of Bachelor's, Master's and Doctoral degree programmes for students.<br> For example, the College of Business and Management, the College of Education and Leadership, the College of Arts and Sciences, and the College of Nursing and Health Sciences, etc.
      </p>
    </div>
  </div>
  <UContainer>
    <UPageBody>

      <div class="program-grid">
        <div v-for="program in programs" :key="program.id" class="program-card">
          <div class="program-image-container">
            <img :src="program.image.src" :alt="program.title" class="program-image">
          </div>
          <div class="program-content">
            <h2 class="program-title">{{ program.title }}</h2>
<!--            <p class="program-description">{{ program.description }}</p>-->
          </div>
        </div>
      </div>

    </UPageBody>
  </UContainer>
  <p class="college-info">
  Holy Family College also accelerated evening classes are offered at the main campus in Manitowoc and at outreach locations in Wisconsin for students who are pursuing an associate's degree at the baccalaureate or graduate level. Courses also include academic advising and credit for prior learning. Other available courses include teacher certification and certificate programmes ranging from business to ministry to social work.
  <br><br>
  Holy Family College prides itself on its highly qualified and experienced administrative and teaching staff in a variety of professional fields, with more than 40,000 alumni globally recognised for their leadership roles in business, healthcare organisations, corporations, educational institutions, entrepreneurial ventures, and non-profit organisations.
</p>
</template>

<style>
.program-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.program-card {
  background-color: white;
  border-radius: 8px;
  overflow: hidden;
  //box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  display: flex;
  flex-direction: column;
  height: 500px; /* 固定卡片高度 */
}

.program-card:hover {
  transform: translateY(-5px);
}

.program-image-container {
  height: 90%; /* 图片容器占80%高度 */
  overflow: hidden;
}

.program-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 8px;
}

.program-content {
  padding: 10px;
  height: 10%; /* 文字内容占20%高度 */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.program-title {
  font-size: 16px;
  font-weight: bold;
  margin: 0;
  color: #333;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.program-description {
  font-size: 14px;
  color: #666;
  line-height: 1.2;
  margin: 5px 0 0;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

.college-description {
  font-family: 'Roboto', 'Helvetica Neue', sans-serif;
  font-size: 24px;
  line-height: 1.8;
  color: #2c3e50;
  max-width: 1300px;
  margin: 40px auto;
  padding: 20px 40px;
  background-color: #ffffff;
  position: relative;
  overflow: hidden;
  border-bottom: 5px solid #3498db;;
}


.college-description p {
  margin: 0;
  text-align: justify;
  hyphens: auto;
}

.college-description p::first-letter {
  font-size: 3em;
  font-weight: 700;
  float: left;
  line-height: 1;
  padding-right: 15px;
  color: #3498db;
}

@media (max-width: 600px) {
  .college-description {
    font-size: 16px;
    padding: 20px;
    margin: 20px;
  }
}


.college-info {
  font-family: 'Roboto', 'Helvetica Neue', sans-serif;
  font-size: 24px;
  line-height: 1.8;
  color: #2c3e50;
  max-width: 1300px;
  margin: 40px auto;
  padding: 20px 40px;
  background-color: #ffffff;
  position: relative;
  overflow: hidden;
  border-bottom: 5px solid #3498db;
  margin-top: -100px;
}


.college-info p {
  margin: 0;
  text-align: justify;
  hyphens: auto;
}

.college-info p::first-letter {
  font-size: 3em;
  font-weight: 700;
  float: left;
  line-height: 1;
  padding-right: 15px;
  color: #3498db;
}

@media (max-width: 600px) {
  .college-info {
    font-size: 16px;
    padding: 20px;
    margin: 20px;
  }
}

</style>
