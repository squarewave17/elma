<template>
  <div id="app">
    <!-- When the emit event fires on the header, showQuiz data is set to true -->
    <Header @startQuiz="showQuiz = true" />
    <!-- v-if conditionally renders the element based on a condition. In our case, when showQuiz is true -->
    <Quiz v-if="showQuiz" />
  </div>
</template>

<script setup>
// This is the script setup syntax - the way forward ;)
import Header from '@/components/Header.vue'
import Quiz from '@/components/Quiz.vue'
// Importing ref from vue - this is a method of storing reactive data
import { ref } from 'vue'
// Create a Boolean ref - this is what quiz looks at to see if it should be showing
const showQuiz = ref(false)
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
@font-face {
  font-family: 'Nunito';
  src: url(./assets/fonts/Nunito/static/Nunito-Regular.ttf);
}
@font-face {
  font-family: 'Rubik';
  src: url(./assets/fonts/Rubik/static/Rubik-Regular.ttf);
}
</style>
