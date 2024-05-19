/**
* @file App.vue
* @description The main component of the Vue.js application.
*/
<template>
<app-form />
</template>


<script>
import AppForm from './components/Form.vue'
export default {
  name: 'App'
}
components: {
  AppForm
}
</script>
