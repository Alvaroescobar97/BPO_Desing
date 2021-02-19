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
                        <router-link active-class="act" to="/home" class="nav-link rounded-3 hover me-1">Inicio</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link active-class="act" to="/about" class="nav-link rounded-3 hover me-1">¿Quiénes Somos?</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/" class="nav-link rounded-3 hover me-1">Portafolio</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/" class="nav-link rounded-3 hover me-1">Servicios</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/" class="nav-link rounded-3 hover me-1">Contacto</router-link>
                    </li>
                </ul>
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link hover login" href="#"><i class="fas fa-sign-out-alt"></i> Login</a>
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
    .hover:hover, .act{
        border: 1px solid #212529;
        background-color: #f8f9fa;
        color: #212529!important;
    }
    
    .login {
        border: 1px solid #212529;
        border-radius: 15px;
        background-color: #212529;
        color: #f8f9fa!important;
    }
    
    .size {
        width: 40px;
        height: 30px;
    }
</style>