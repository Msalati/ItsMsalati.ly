<template>
  <div>
    <nav-bar />
    <div class="circle-parent">
      <div class="circle">

      </div>
    </div>
  </div>
</div></template>

<script>
import NavBar from "~/components/NavBar.vue";

export default {
  name: "IndexPage",
  components: { NavBar },
};
</script>
<style>
@import url("../assets/css/style.css");

h1 {
  text-align: center;
}

.circle-parent {

  display: flex;
  justify-content: center;
}

.circle {
  background: linear-gradient(45deg, #000000, #3DF2F2);
  background-size: 400% 400%;
  animation: gradient 2s ease-in infinite;
  border-radius: 50%;
  height: 25vw;
  width: 25vw;
  @media screen and (max-width: 600px) {
    height: 50vw;
    width: 50vw;
  }
}

@keyframes gradient {

  0% {
    background-position: 0% 0%;
  }

  100% {
    background-position: 100% 100%;
  }
}
</style>
