<template>
  <div class="app">
    <global-header />
    <hero-main />
    <filters />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero-main.vue';
import Filters from './components/Filters.vue';

export default {
	name: 'app',
	components: {
		'global-header': Header,
		'hero-main': Hero,
		filters: Filters,
	},
};
</script>

<style lang="scss">
@import './assets/styles/styles';
</style>
