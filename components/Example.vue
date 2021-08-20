<template>
<div>

<div class="label" @click="labelClick">
  laaaabel
</div>
  <button @click="buttonClick">
    ahoj
  </button>
</div>
</template>

<script>
export default {
  methods: {
    labelClick() {
      this.$emit('labelClick')
    },
    buttonClick() {
      this.$emit('buttonClick', {
        name: "jakob",
        age: 22
      })
    }
  }
}
</script>

<style>

</style>
