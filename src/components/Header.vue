 <template>
  <header class="global-header" role="banner">
    <a href="#" class="global-header__branding" role="link"><img src="../assets/img/logo-autosales.svg" alt="Icon of a Yellow Car" class="logo" role="presentation"/><h1 class="global-header__title" role="heading">AutoSales.com</h1></a>
     <section class="global-header__controls u-flex" role="region">
        <button class="search-icon__button" role="button"><img src="../assets/img/icon-search-white.svg" alt="Magnifying Glass Symobolizing a Search Field" class="search-icon__image" role="presentation"></button>
        <button class="global-header__nav-button" @click="toggleNav" role="button">
          <span class="nav-button__icon" :class="{active: isActive}" role="presentation"></span>
        </button>
     </section>
    <nav class="global-header__nav" :class="{'global-header__nav--animated-open': isActive}" role="navigation">
      <ul class="nav-list u-flex" role="list">
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
@import '../assets/styles/styles';
</style>
