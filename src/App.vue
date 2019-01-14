<template>
  <div class="app">
    <Navbar />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
	name: 'app',
	components: {
		Navbar,
	},
};
</script>

<style lang="scss">
@import './assets/styles/styles';
</style>
