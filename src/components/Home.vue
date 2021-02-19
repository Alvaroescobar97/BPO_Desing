<template>
  <div class="container">
    <div class="flex-1">
      <div class="foto-casa rounded-3"></div>

      <div class="informacion-bpo">
        <h1 class="mb-3">BPO <span class="focus">INMOBILIARIA</span></h1>
        <p class="m-0">
          Estamos comprometidos con los inmuebles de nuestros Clientes y
          Aliados. Nuestra asesoría es personalizada y es una actividad diaria
          de cada uno de los integrantes del equipo comercial. Nos encargamos de
          todos los servicios relacionados con la propiedad raíz, como son:
        </p>
        <ul class="mt-3">
          <li>Asesoría en viviendas</li>
          <li>Venta de propiedad Raíz</li>
          <li>Alquiler de propiedad Raíz</li>
        </ul>
        <p class="border-bottom border-2 pb-3 m-0">
          Te asesoramos para que puedas realizar la mejor inversión.
        </p>
        <router-link to="/about" class="btn btn-dark mt-3 py-2 px-3 fw-bold"
          >Leer más...</router-link
        >
      </div>
    </div>

    <div class="flex-2">
      <div class="grid">
        <div class="disenio">
          <a href="">Diseño & Construcción <i class="fas fa-angle-right"></i
          ></a>
        </div>

        <div class="construccion">
          <a href=""
            >Portafólio Arquitectónico <i class="fas fa-angle-right"></i
          ></a>
        </div>

        <div class="foto-1"></div>

        <div class="foto-2"></div>

        <div class="contacto-asesor">
          <h2>Contacta con un Asesor Comercial</h2>
          <h3>Llama a las lineas:</h3>
          <p class="mt-3 align-middle fs-3"><i class="fs-3 fas fa-phone-alt me-3 telefono"></i>310 419 63 48 - 320 776 49 32</p>
        </div>
      </div>

      <div class="foto-jardin"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style>
.focus {
  color: #ee1b24;
}

.flex-1 {
  margin-top: 3rem;
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: space-between;
  margin-bottom: 2rem;
}

.flex-2 {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: space-between;
  margin-bottom: 3rem;
}

.foto-casa {
  flex-basis: calc(70% - 1rem);
  background-image: url(../assets/1.jpeg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  margin-bottom: 2rem;
  min-height: 500px;
}

.informacion-bpo {
  flex-basis: calc(30% - 1rem);
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, 1fr);
  flex-basis: calc(70% - 1rem);
}

.foto-jardin {
  flex-basis: calc(30% - 1rem);
  background-image: url(../assets/2.jpg);
  background-size: cover;
  background-position: center center;
  min-height: 500px;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}

.disenio {
  grid-row: 1/2;
  grid-column: 1/4;
  background-color: black;
  text-align: center;
  min-height: 30px;
  border-top-left-radius: 5px;
  padding: 10px;
}

.disenio a {
  color: white;
  text-decoration: none;
  font-size: 1.5rem;
}

.construccion {
  grid-row: 1/2;
  grid-column: 4/6;
  background-color: black;
  text-align: center;
  border-top-right-radius: 5px;
  padding: 10px;
}

.construccion a {
  color: white;
  text-decoration: none;
  font-size: 1.5rem;
}

.foto-1 {
  grid-row: 2/3;
  grid-column: 1/4;
  background-image: url(../assets/foto-1.jpg);
  background-size: cover;
  background-position: center center;
  min-height: 450px;
}

.foto-2 {
  grid-row: 2/3;
  grid-column: 4/6;
  background-image: url(../assets/foto-2.png);
  background-size: cover;
  background-position: center left;
  min-height: 450px;
}

.contacto-asesor {
  padding: 2rem 0rem;
  grid-row: 3/4;
  grid-column: 1/6;
  text-transform: uppercase;
  text-align: center;
  background-color: black;
  color: white;
}

.telefono{
  background-color: #ee1b24;
  text-align: center;
  padding: 12px 8px;
  width: 55px;
  border-radius: 50%;
  border: 2px solid white;
}

@media (min-width: 992px) {
  .flex-1 {
    flex-direction: row;
  }
  .foto-casa {
    margin-bottom: 0rem;
  }
  .flex-2 {
    flex-direction: row;
  }
  .contacto-asesor{
    
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
  }
  .foto-jardin{
    border-bottom-left-radius: 0px;
  }
}
</style>