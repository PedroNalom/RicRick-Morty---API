<template>
  <div class="container">
  <div id="carouselExampleDark" class="carousel carousel-dark slide">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleDark" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active" data-bs-interval="10000">
      <img src="https://image.tmdb.org/t/p/original/vDPXV2VqzeALc7WVnOetzS1xQQ7.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h6>About Me</h6>
        <p>Meu nome é Pedro Henrique Nalom, tenho 19 anos. Atualmente estou cursando Analise e Desenvolvimento de Sistema na Unimar. Meu Registro de Aluno é 1968133 e atualmente estou no terceiro termo da turma C.   </p>
      </div>
    </div>
    <div class="carousel-item" data-bs-interval="2000">
      <img src="https://th.bing.com/th/id/OIP.ZeIPPzntkZcFf2qir9aHdwHaDq?rs=1&pid=ImgDetMain" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h6>Hard Skils</h6>
        <p>Domínio de HTML e CSS intermediário, contando com PHP e Python para o desenvolvimento de projetos. Em desenvolvimento de skils nas áreas citadas e em específico JS.  </p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="https://th.bing.com/th/id/OIP.X7fFEohYCahFGKwwSFnCFAAAAA?rs=1&pid=ImgDetMain" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h6>Soft Skils</h6>
        <p>Boa comunicação, facilidade de relação entre pessoas, proatividade, participação e facilidade em trabalhar em equipe.  </p>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
</div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
  .container {
    max-width: 800px; 
    margin: 0 auto; 
    border: 1px solid #ccc; 
    padding: 20px; 
  } 
  P, h6{
    background-color: #ccc;
  }
  
}
</style>
