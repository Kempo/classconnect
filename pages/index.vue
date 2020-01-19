<template>
  <div class="container">
    <div>
      <img src="~/assets/Group 3.svg" class="logo" height="100" alt="logo" />
      <h2 class="subtitle">
        Connect Schools.Connect Classrooms.Connect Students.
      </h2>
    </div>
    <div>
      <b-button variant="success" class="btn" href="/explore">Connect</b-button>
    </div>
  </div>
</template>

<script></script>

<style>
body {
  font-family: Product Sans Medium, sans-serif;
  background-color: #e5e5e;
}

.logo {
  animation: fadeIn ease 3s;
  margin-left: 315px;
  margin-top: 175px;
  margin-bottom: 50px;
}

.subtitle {
  animation: fadeIn ease 7s;
  margin-left: 160px;
}

.btn {
  margin-left: 510px;
  margin-top: 30px;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
