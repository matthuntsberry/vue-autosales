<template>
  <div class="app">
    <global-header />
    <hero-main />
    <filters />
    <featured />
    <global-footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero-main.vue';
import Filters from './components/Filters.vue';
import Featured from './components/Featured-Content__Card.vue';
import Footer from './components/Footer.vue';

export default {
	name: 'app',
	components: {
		'global-header': Header,
		'hero-main': Hero,
		filters: Filters,
		featured: Featured,
		'global-footer': Footer,
	},
};
</script>

<style lang="scss">
@import './assets/styles/styles';
</style>
