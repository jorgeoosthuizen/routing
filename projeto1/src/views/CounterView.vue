<script setup>
    import {useCounterStore} from '@/stores/counter'
    const counter =useCounterStore()

</script>
<template>
  <div class="about">
    <h1>This is an app Counter page</h1>
    <button @click="counter.increment()">Clique aqui para incrementar</button> 
    <p>O valor do contador e {{ counter.count }}</p>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>