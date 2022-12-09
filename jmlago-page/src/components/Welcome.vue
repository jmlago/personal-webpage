<script setup lang="ts">
defineProps<{
  msg: string;
}>();
</script>

<template>
  <div class="centered">
  <div class="greetings">
    <h1 class="orange1">{{ msg }}</h1>
    <h3 class="purple1">
      I'm 
      <a class="orange1" href="https://twitter.com/josemlago" target="_blank" rel="noopener">@josemlago</a>,
       a micro-freelancer and indie hacker!
    </h3>
    <h2 class="purple1">
      Select with arrows and press enter
    </h2>
  </div>
  <div class="menu">
    <RouterLink class="orange1 menu" to="/gigs">Gigs that I offer</RouterLink>
  </div>
  <div class="menu">
    <RouterLink class="purple1 menu" to="/projects">Projects that I'm involved</RouterLink>
  </div>
  <div class="menu">
    <RouterLink class="purple1 menu" to="/mystory">My story</RouterLink>
  </div>
</div>
</template>

<style scoped>
h1 {
  font-family: "broken-console-bold";
  font-size: 7rem;
}

h3 {
  font-family: "broken-console";
  font-size: 2rem;
}
h2 {
  font-family: "broken-console-bold";
  font-size: 3rem;
  top: 10px;
}

.menu {
  text-align: center;
  font-family: "broken-console";
  font-size: 2rem;
  top: 20px;
}
.menu div{
  text-align: center;
}
.greetings h1,
.greetings h3 {
  text-align: center;
}
.greetings h2 {
  text-align: center;
}

.centered {
  top: 60%;
  text-align: center;
}
@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
  .greetings h2 {
    text-align: center;
  }
}
</style>
