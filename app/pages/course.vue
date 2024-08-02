<script setup lang="ts">

</script>

<template>
  <img class="imageplaceholder" src="/Class_c.jpg" >
  <div class="div1">
    <h1>Undergraduate major</h1>
    <div class="major-container">
      <div class="major-category">
        <h2>Business</h2>
        <ul>
          <li>Business administration</li>
          <li>finance</li>
          <li>Human resource management</li>
          <li>Enterprise management</li>
          <li>marketing</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Education</h2>
        <ul>
          <li>Early Childhood Education</li>
          <li>Educational Administration</li>
          <li>Pedagogy</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Engineering</h2>
        <ul>
          <li>Mechanical engineering</li>
          <li>Electrical engineering</li>
          <li>Computer engineering</li>
          <li>Civil engineering</li>
          <li>Chemical engineering</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Economics</h2>
        <ul>
          <li>economics</li>
          <li>finance</li>
          <li>statistics</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Science</h2>
        <ul>
          <li>biology</li>
          <li>environmental science</li>
          <li>mathematics</li>
          <li>physics</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Humanities</h2>
        <ul>
          <li>philosophy</li>
          <li>psychology</li>
          <li>sociology</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Art</h2>
        <ul>
          <li>graphic design</li>
          <li>Industrial design</li>
          <li>Visual communication design</li>
          <li>Interior design</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>Foreign Languages</h2>
        <ul>
          <li>Chinese</li>
          <li>Russian</li>
          <li>Spanish</li>
          <li>French</li>
          <li>Korean</li>
          <li>Japanese</li>
          <li>German</li>
        </ul>
      </div>
      <div class="major-category">
        <h2>International Relations</h2>
        <ul>
          <li>International political economy</li>
          <li>International environmental development</li>
          <li>International development</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="div2">
    <h1>Graduate major</h1>

    <div class="major-container">
      <div class="major-category">
        <h2>Business</h2>
        <ul>
          <li>Business administration</li>
          <li>Human resource management</li>
          <li>Enterprise management</li>
          <li>marketing</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Law</h2>
        <ul>
          <li>Law Practice</li>
          <li>International Law</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Engineering</h2>
        <ul>
          <li>Mechanical engineering</li>
          <li>Electrical engineering</li>
          <li>Computer engineering</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Economics</h2>
        <ul>
          <li>economics</li>
          <li>finance</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Science</h2>
        <ul>
          <li>biology</li>
          <li>mathematics</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Humanities</h2>
        <ul>
          <li>philosophy</li>
          <li>sociology</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Art</h2>
        <ul>
          <li>graphic design</li>
          <li>Industrial design</li>
          <li>Visual communication design</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Foreign Languages</h2>
        <ul>
          <li>Chinese</li>
          <li>Russian</li>
          <li>Spanish</li>
          <li>French</li>
          <li>Korean</li>
          <li>Japanese</li>
          <li>German</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>International Relations</h2>
        <ul>
          <li>International environmental development</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="div3">
    <h1>Doctoral major</h1>

    <div class="major-container">
      <div class="major-category">
        <h2>Business</h2>
        <ul>
          <li>Business administration</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Law</h2>
        <ul>
          <li>Law Practice</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>International Relations</h2>
        <ul>
          <li>International environmental development</li>
        </ul>
      </div>

      <div class="major-category">
        <h2>Foreign Languages</h2>
        <ul>
          <li>Chinese</li>
          <li>Russian</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
.imageplaceholder {
  width: 1920px;
}
.div1 {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}
.div2 {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.div3 {
   font-family: Arial, sans-serif;
   line-height: 1.6;
   color: #333;
   max-width: 1200px;
   margin: 0 auto;
   padding: 20px;
 }

h1 {
  text-align: center;
  color: #2c3e50;
  font-size: 30px;
  font-weight: bolder;
  margin-bottom: 10px;
}

.major-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.major-category {
  width: 30%;
  margin-bottom: 30px;
}
.major-category h2 {
  color: #2980b9;
  border-bottom: 2px solid #3498db;
  padding-bottom: 5px;
}
ul {
  list-style-type: none;
  padding-left: 0;
}
li {
  margin-bottom: 5px;
}
</style>
