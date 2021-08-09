<template>
  <button @click="handleClick">Button</button>
</template>

<script>
export default {
  name: 'Button',
  emits: {
    submit: (number) => number < 10
  },
  methods: {
    handleClick() {
      this.$emit('submit', 10)
    }
  }
}
</script>

<style>

</style>