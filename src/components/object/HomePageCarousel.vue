<template>
  <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
        aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
        aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
        aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner ratio ratio-16x9">
      <div class="carousel-item active">
        <img src="/src/assets/img/Carousel1.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="/src/assets/img/Carousel2.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="/src/assets/img/Carousel3.png" class="d-block w-100" alt="...">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
      <div class="carousel-control-prev-icon" aria-hidden="true">
        <i class="bi bi-chevron-left text-dark position-absolute top-50 start-50 translate-middle"></i>
      </div>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" typ e="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
      <div class="carousel-control-next-icon" aria-hidden="true">
        <i class="bi bi-chevron-right text-dark position-absolute top-50 start-50 translate-middle"></i>
      </div>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script setup>
</script>

<style scoped>
.carousel .carousel-indicators button {
  width: 10px;
  height: 10px;
  border-radius: 100%;
  background-color: black;
}

.carousel-indicators {
  bottom: -50px;
}

.carousel-control-prev-icon,
.carousel-control-next-icon {
  height: 2rem;
  width: 2rem;
  outline: white;
  background-size: 100%, 100%;
  border-radius: 50%;
  border: 1px solid white;
  background-color: white;
  background-image: none;
}
</style>