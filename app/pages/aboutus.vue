<script setup lang="ts">

</script>

<template>
  <div class="about-us-container">

    <div class="content-section">

      <div class="text-block">
        <h1>Our History</h1>
        <p>Holy Family College traces its history to 1885 when the Franciscan Sisters of Christian Charity established Holy Family Academy and Normal School to prepare young women who entered the religious community for teaching. They founded Holy Family College in 1935. The college began admitting lay women in 1957 and became coeducational in 1969. 
<br><br>
          The college was located in a wing of Holy Family Convent for 25 years. In the late 1950s, a capital campaign was launched to build a new college building on 36 acres adjacent to Holy Family Convent. The new Holy Family College building opened in 1960. In 1972 the college became separately incorporated from the Franciscan order, and was renamed Silver Lake College of the Holy Family.
          <br><br>
          During the late 1970s and early 1980s, Silver Lake College of the Holy Family expanded programs to nontraditional students. Beginning in the mid-1980s, the college also offered degree-completion programs and professional development coursework.
          <br><br>
          George F. Arnold was appointed the college's first lay president and served from 2004 to 2013.
          <br><br>
          Clare Hall was renovated to offer on-campus student housing in 2009.
          <br><br>
          Dr. Robert B. Callahan became Holy Family College's 11th president in 2018.
          <br><br>
          In September 2019, Silver Lake College announced that it would be renamed Holy Family College, and established different branches, in a return to its Franciscan roots.</p>
      </div>

      <div class="image-divider">
        <img src="/history.jpg" alt="Historical photo of Holy Family College" />
      </div>

    </div>
  </div>
</template>

<style scoped>
.about-us-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  font-family: Arial, sans-serif;
}


.hero-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.content-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  font-size: 2.5em;
  color: #333;
  margin-bottom: 40px;
  text-align: center;
}

.text-block {
  width: 100%;
  max-width: 800px;
  margin-bottom: 40px;

}

.text-block h2 {
  font-size: 2em;
  color: #333;
  margin-bottom: 20px;
  text-align: center;
}

.text-block p, .text-block ul {
  font-size: 1.1em;
  color: #555;
  line-height: 1.6;
}

.text-block ul {
  padding-left: 20px;
}

.image-divider {
  width: 100%;
  height: 300px;
  overflow: hidden;
  margin-bottom: 40px;
}

.image-divider img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

@media (max-width: 768px) {
  .hero-image {
    height: 200px;
  }

  .image-divider {
    height: 200px;
  }

  h1 {
    font-size: 2em;
  }

  .text-block h2 {
    font-size: 1.5em;
  }

  .text-block p, .text-block ul {
    font-size: 1em;
  }
}
</style>
