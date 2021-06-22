<template>
  <button @click="contador++">Aumentar</button>
  <button @click="disminuir">Disminuir</button>
</template>

<script>
import { inject } from '@vue/runtime-core'
export default {

    setup(){
      const contador = inject('contador');

      //Metodos
      const disminuir = ()=>{
        contador.value --;

      }
      return {contador,disminuir}
    }
}
</script>

<style>

</style>