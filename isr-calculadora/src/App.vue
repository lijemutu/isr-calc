<script setup>
import HeroTitle from './components/HeroTitle.vue'
import Calculator from './components/Calculator.vue'
import Instructions from './components/Instructions.vue'
import Results from './components/Results.vue'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" /> -->

    <div class="">
      <HeroTitle></HeroTitle>
    </div>
  </header>

  <main>
    <Calculator></Calculator>
    <Instructions></Instructions>
    <Results></Results>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}



@media (min-width: 1024px) {
  header {
    display: block;
    padding-right: calc(var(--section-gap) / 2);
  }


}
</style>
