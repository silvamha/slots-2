/**
* @file App.vue
* @description The main component of the Vue.js application.
*/
<template>
  <app-form>
    <div class="help">
      <p>This is some help text.</p>
    </div>
    <div class="fields">
      <input type="text" placeholder="email">
      <input type="text" placeholder="admin">
      <input type="password" placeholder="password">
    </div>
    <div class="buttons">
      <button type="submit">Submit</button>
    </div>
  </app-form>
  <app-form>
    <div class="help">
      <p>Contact help text.</p>
    </div>
    <div class="fields">
      <input type="text" placeholder="name">
      <input type="text" placeholder="message">
    </div>
    <div class="buttons">
      <button type="submit">Submit</button>
    </div>
  </app-form>
</template>


<script>
import AppForm from './components/Form.vue'

export default {
  name: 'App',
  components: {
    AppForm,
  }
}
</script>
