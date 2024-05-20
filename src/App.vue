/**
* @file App.vue
* @description The main component of the Vue.js application.
*/

<template>
  <app-form>
    <!-- Slot for help text -->
    <template v-slot:help>
      <p>{{ help }}</p>
    </template>
    <!-- Slot for form fields -->
    <template v-slot:fields>
      <input type="text" placeholder="email">
      <input type="text" placeholder="admin">
      <input type="password" placeholder="password">
    </template>
    <!-- Slot for buttons -->
    <template v-slot:buttons>
      <button type="submit">Submit</button>
    </template>
    <p>Dummy Text</p>
  </app-form>
  <app-form>
    <!-- Slot for help text -->
    <template v-slot:help>
      <p>Contact help text.</p>
    </template>
    <!-- Slot for form fields -->
    <template v-slot:fields>
      <input type="text" placeholder="name">
      <input type="text" placeholder="message">
    </template>
    <!-- Slot for buttons -->
    <template v-slot:buttons>
      <button type="submit">Submit</button>
    </template>
  </app-form>
</template>


<script>
import AppForm from './components/Form.vue'

export default {
  name: 'App',
  components: {
    AppForm,
  },
  data() {
    return {
      help: 'This is some help text.',
    }
  }
}
</script>
