<template>
 <ExampleComponent/>
</template>

<style>
.nuxt-logo {
  height: 180px;
}
</style>

<script lang="ts">
import Vue from 'vue'
import ExampleComponent from './Example.vue'
export default Vue.extend({
  components: {ExampleComponent},
  methods: {
    alertino: (co) => {
      alert(co)
    }
  }
})
</script>
