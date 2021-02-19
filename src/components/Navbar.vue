<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light container-fluid">

        <div class="container">
            <a class="navbar-brand" href="#"><img class="size" src="../assets/logo-without-letters.png" alt=""></a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse text-center" id="navbarNavDropdown">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <router-link to="/home" class="nav-link rounded-3 hover">Inicio</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/about" class="nav-link rounded-3 hover">¿Quiénes Somos?</router-link>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link rounded-3 hover" href="#">Portafolio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link rounded-3 hover" href="#">Servicios</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link rounded-3 hover" href="#">Contacto</a>
                    </li>
                </ul>
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link rounded-3 hover" href="#"><i class="fas fa-sign-out-alt"></i> Login</a>
                    </li>
                </ul>
            </div>

        </div>
    </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style>

    .hover:hover {
        background-color: #ccc;
    }

    .size {
        width: 40px;
        height: 30px;
    }
</style>