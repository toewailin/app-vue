<template>
    <header>
        <h1>Hello from {{ title }}</h1>
        <Button />
    </header>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: 'AppHeader',
  props: {
    title: {
      type: String,
      default: 'Task Tracker',
    },
  },
  components: {
    Button
  },
}
</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

/* Add any additional styles specific to this component */
</style>
