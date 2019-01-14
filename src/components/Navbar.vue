 <template>
  <header class="global-header" role="banner">
    <a href="#" class="global-header__title"><img src="../assets/images/logo-autosales.svg" alt="Icon of a Yellow Car" class="logo"/>AutoSales.com</a>
    <nav class="global-header__nav" role="navigation">
      <ul class="nav-list" role="list">
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Cars for Sale</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Sell My Car</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Find a Dealer</a></li>
        <li class="nav-list__item" role="listitem"><a href="#" class="nav-list__link" role="link">Contact Us</a></li>
        <li class="nav-list__item" role="listitem"><span><img src="../assets/images/icon-search-white.svg" alt="Magnifying Glass Symobolizing a Search Field" class="search-icon"></span></li>
      </ul>
    </nav>    
  </header>
</template>

<script>
export default {
	name: 'Navbar',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/styles/styles';
</style>
