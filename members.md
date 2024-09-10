---
layout: page
title: Lab members
subtitle: 
---

<style>
.member-photo {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 10px;
}
.member-container {
  margin-bottom: 30px;
  height: 220px; /* Adjust this value as needed */
}
.member-name {
  display: block;
  text-align: center;
  word-wrap: break-word;
  width: 100%;
}
</style>

### Faculty

<div class="container-fluid">
  <div class="row">
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/oliver_kroemer_.jpg" alt="Oliver Kroemer" />
      <a class="member-name" href="https://www.ri.cmu.edu/ri-faculty/oliver-kroemer/">Oliver Kroemer</a>
    </div>
  </div>
</div>

### PhD Students

<div class="container-fluid">
  <div class="row">
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/kevin_zhang_.jpg" alt="Kevin Zhang" />
      <a class="member-name" href="https://www.linkedin.com/in/shashwat-1singh/">Kevin Zhang</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/saumya_saxena_.jpg" alt="Saumya Saxena" />
      <a class="member-name" href="https://www.linkedin.com/in/shashwat-1singh/">Saumya Saxena</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/alex_lagrassa_.jpg" alt="Alex Lagrassa" />
      <a class="member-name" href="https://www.linkedin.com/in/shashwat-1singh/">Alex Lagrassa</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/mark_lee_.jpg" alt="Mark Lee" />
      <a class="member-name" href="https://si-lynnn.github.io/">Mark Lee</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/yunus_seker.jpg" alt="Yunus Seker" />
      <a class="member-name" href="https://si-lynnn.github.io/">Yunus Seker</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/zilin_si_.jpg" alt="Zilin Si" />
      <a class="member-name" href="https://si-lynnn.github.io/">Zilin Si</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/sarvesh_.jpg" alt="Sarvesh Patil" />
      <a class="member-name" href="https://servo97.github.io/">Sarvesh Patil</a>
    </div>
  </div>
</div>

### Master's Students

<div class="container-fluid">
  <div class="row">
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/xinyu_wang_.jpg" alt="Xinyu Wang" />
      <a class="member-name" href="https://snibo.me">Xinyu Wang</a>
    </div>
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/janice_lee.png" alt="Janice Lee" />
      <a class="member-name" href="https://snibo.me">Janice Lee</a>
    </div>
  </div>
</div>

### Undergraduate students

<div class="container-fluid">
  <div class="row">
    <div class="col-md-3 text-center member-container">
      <img class="member-photo" src="../img/members/lawrence_feng.jpeg" alt="Lawrence Feng" />
      <a class="member-name" href="https://snibo.me">Lawrence Feng</a>
    </div>
  </div>
</div>

## Alumni

- [Jacky Liang](http://www.edayaxin.com/) (Ph.D 2023, Google)
- [Mohit Sharma](http://www.edayaxin.com/) (Ph.D 2024, Google)
- [Shivam Vats](http://www.edayaxin.com/) (Ph.D 2024, Brown)
- [Tabitha Lee](http://www.edayaxin.com/) (Ph.D 2024, Lockheed Martin)
<hr>
- [Eric Zhang](http://www.edayaxin.com/) (M.S 2022, UIUC)
- [Eric Zhang](http://www.edayaxin.com/) (M.S 2022, UIUC)
<hr>
- [Fabian H](http://www.edayaxin.com/) (RISS intern 2024, University H.)
- [Fabian H](http://www.edayaxin.com/) (RISS intern 2024, University H.)

<style>
/* Added styles for the slideshow */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}
.slideshow-image {
  width: 100%;
  height: 400px;
  object-fit: cover;
  display: none;
  opacity: 0;
  transition: opacity 0.5s ease-in-out;
}
.slideshow-image.active {
  display: block;
  opacity: 1;
}
</style>

## Some IAM Joyful Moments


<div class="slideshow-container">
  <img class="slideshow-image" src="../img/lab/lab_pic_11_16_2019.jpg" alt="Lab Photo 1">
  <img class="slideshow-image" src="../img/lab/lab_pic_5_1_2019.jpg" alt="Lab Photo 2">
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const images = document.querySelectorAll('.slideshow-image');
  let currentIndex = 0;

  function nextSlide() {
    images[currentIndex].classList.remove('active');
    currentIndex = (currentIndex + 1) % images.length;
    images[currentIndex].classList.add('active');
  }

  setInterval(nextSlide, 3000); // Change slide every 3 seconds
});
</script>
