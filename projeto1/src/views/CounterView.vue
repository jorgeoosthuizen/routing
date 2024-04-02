<template>
    <div class="about">
      <h1>This is the counter page</h1>
      <button @click="counter.increment()"> Clique para incrementar</button>
      <p>O valor do contador é {{ counter.count }}</p>
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

  <script>
  import {useCounterStore} from '@/stores/counter'
  const counter = useCounterStore()
</script>