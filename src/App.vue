<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
	<TestComponent str="My first component wow i like VUE"></TestComponent>

	<h1>test slider</h1>
	<MySlider @click="handleClick"></MySlider>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import TestComponent from './components/TestComponent.vue'
import MySlider from './components/MySlider.vue'

export default {
  name: 'App',
  components: {
		TestComponent,
		MySlider
    // HelloWorld
  }
}
</script>