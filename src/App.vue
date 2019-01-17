<template>
  <div class="app">
    <global-header />
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
	name: 'app',
	components: {
		'global-header': Header,
	},
};
</script>

<style lang="scss">
@import './assets/styles/styles';
</style>
