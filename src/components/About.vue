<template>
  <div class="container">
    <div class="d-flex my-3 flex-sm-column flex-lg-row flex-xs">
      <div class="align-self-center me-3">
        <h2 class="text-center mb-5">¿Quiénes Somos?</h2>
        <p class="justify">
          Somos una empresa BPO (Business Process Outsourcing – Negocios
          procesos externos) promotora del sector inmobiliario y constructor,
          conformada por un grupo de profesionales éticos, capacitados y
          comprometidos en la estructura de proyectos y negocios, con el fin de
          generar seguridad y confianza a nuestros clientes y la mejor
          oportunidad de hacer excelente relaciones comerciales con nuestra
          plataforma de servicios con aliados competitivos.
        </p>
      </div>
      <img
        class="img-size rounded-3"
        src="../assets/teamwork.jpg"
        alt="Team Work"
      />
    </div>

    <div class="">
      <h2 class="text-center">Nuestro Equipo</h2>

      <div class="lista-equipo">

        <div class="miembro-equipo">
          <img src="../assets/equipo/canito.jpg" alt="Miembro Equipo" />
          <p>Esteban Cano A.</p>
        </div>

        <div class="miembro-equipo">
          <img src="../assets/equipo/nathalie.jpg" alt="Miembro Equipo" />
          <p>Nathalie Ospina A.</p>
        </div>

        <div class="miembro-equipo">
          <img src="../assets/equipo/melosky.jpg" alt="Miembro Equipo" />
          <p>Alvaro Escobar</p>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style>
.flex-xs {
  flex-direction: column;
}
.justify {
  text-align: justify;
}
.img-size {
  max-width: 480px;
}
@media (min-width: 480px) {
  .img-size {
    max-width: 680px;
  }
}
@media (min-width: 920px) {
  .img-size {
    max-width: 700px;
  }
}

/*Equipo*/

/*
.lista-equipo {
  list-style: none;
  padding: 0;
}

.lista-equipo li {
  padding: 1rem;
  float: left;
  max-width: 307px;
}

@media (min-width: 812px) {
  .lista-equipo li {
    width: 50%;
  }
}

@media (min-width: 992px) {
  .lista-equipo li {
    width: 33.3%;
  }
}
*/

.lista-equipo {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: space-between;
  justify-content: center;
  align-items: center;
}

@media (min-width: 812px) {
  .lista-equipo{
    flex-direction: row;
  }
  .miembro-equipo{
    flex-basis: calc(50% - 1rem);
  }
}

@media (min-width: 992px) {
  .miembro-equipo{
    flex-basis: calc(33.3% - 1rem);
  }
}

.miembro-equipo {
  position: relative;
  overflow: hidden;
  max-width: 328px;
  text-align: center;
  margin: 10px;
}

.miembro-equipo img {
  height: 410px;
  filter: gray;
  -webkit-filter: grayscale(1);
  -webkit-transition: all 0.5s ease-in-out;
}

.miembro-equipo:hover img {
  -webkit-transform: scale(1.2);
  -webkit-filter: grayscale(0);
  /*transform: rotate(3deg);*/
}

.miembro-equipo p {
  position: absolute;
  bottom: 0;
  left: 0;
  margin-bottom: 0px;
  padding: 10px 10px 10px 10px;
  background-color: rgba(0, 0, 0, 0.7);
  width: 100%;
  text-align: center;
  color: #ee1b24;
  text-transform: uppercase;
  font-weight: bold;
  -webkit-transition: all 0.5s ease-in-out;
}

.miembro-equipo:hover p {
  bottom: -80px;
  opacity: 0;
}
</style>