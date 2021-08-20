<template>
<ExampleComponent @labelClick="printIntoAlert"  @buttonClick="printIntoAlert" />
</template>

<script lang="js">
import Vue from 'vue'
import ExampleComponent from '~/components/Example.vue'

export default Vue.extend({
  components: { ExampleComponent }, methods: {
    printIntoAlert: (subject = null) => {
      if (!subject) {
        alert('stalo sa ')
      } else {
        alert(`Ahoj ${subject.name} mas ${subject.age} rokov`)
      }
    }
  }})
</script>
