<template>
  <footer class="bg-dark text-white text-center p-4">
    <p class="m-0">BPO - Todos los Derechos Reservados - 2021 &copy;</p>
    <p class="m-0"><i class="fas fa-phone-alt me-2"></i> 3104196348 - 3156705421 | <i class="fab fa-google mx-2"></i> proyectosbpobroker@gmail.com</p>
    <ul class="icons">
            <li><i class="fab fa-facebook-f"></i></li>
            <li><i class="fab fa-instagram"></i></li>
            <li><i class="fab fa-whatsapp"></i></li>
    </ul>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style>
.icons {
  display: flex;
  list-style: none;
  justify-content: left;
  padding: 10px 0;
  margin: 0;
  color: white;
  justify-content: center;
}
.icons li {
    display: block;
    margin-right: 15px;
}
</style>