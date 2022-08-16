<template>
  <div>
    <h2>2: Counting the Number of Characters</h2>
    <p>What is the input string? </p>
    <input v-model="text" placeholder="Homer"/>
    <span>{{ nameLength() }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'VueSolution002',
  data() {
    return {
      text: ''
    }
  },
  methods: {
    reverse: function() {
      this.text = this.text.split('').reverse().join('');
    },
    nameLength: function() {
      return this.text.length;
    }
  }
});
</script>