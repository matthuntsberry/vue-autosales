 <template>
  <header class="global-header" role="banner">
    <a href="#" class="global__branding u-grid" role="link">
      <img src="../assets/img/logo-autosales.svg" alt="Animated Yellow Car" class="logo" role="presentation"/>
      <h1 class="global__title" role="heading">AutoSales.com</h1>
    </a>
     <section class="global-header__controls u-grid" role="region">
        <button class="global-search__button" role="button"><img src="../assets/img/icon-search-white.svg" alt="Magnifying Glass Symobolizing a Search Field" class="global-search__icon" role="presentation"></button>
        <button class="global-nav__button" @click="toggleNav" role="button">
          <span class="global-nav__button-icon" :class="{'nav--active': isActive}" role="presentation"></span>
        </button>
     </section>
    <nav class="global-nav" :class="{'global-nav__button--animated-open': isActive}" role="navigation">
      <ul class="nav-list u-grid" role="list">
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Cars for Sale</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Sell My Car</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Find a Dealer</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Contact Us</a></li>
      </ul>
    </nav>   
  </header>
</template>

<script>
export default {
	name: 'global-header',
	data() {
		return {
			isActive: false,
		};
	},
	methods: {
		toggleNav() {
			this.isActive = !this.isActive;
		},
	},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
