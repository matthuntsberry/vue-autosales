<template>
  <main class="feature-content" role="main">
  <section class="featured-content__card u-grid" role="region" v-for="(product, index) in products" :key="index">
    <section class="card-content__text" role="region">
      <h2 class="card__title" role="heading">{{product.title}}</h2>
      <p class="card__body">{{product.description}}</p>
      <a href="#" class="card__button">View All</a>
    </section>
    <section class="card-content__images" role="region">
      <a href="#" role="link">
        <picture class="card__image-container" v-for="(img, index) in product.img" :key="index">
          <img class="card__image" v-bind:src="img" role="img"/>
        </picture>
      </a> 
    </section>    
  </section>
  </main>
</template>

<script>
export default {
	data() {
		return {
			products: [
				{
					title: 'Honda Cars and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-honda-car.jpg',
						'/img/img-card-landing-med-honda-suv.jpg',
					],
				},
				{
					title: 'Audi Cars and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-audi-car.jpg',
						'/img/img-card-landing-med-audi-suv.jpg',
					],
				},
				{
					title: 'Chevy Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-chevy-car.jpg',
						'/img/img-card-landing-med-chevy-suv.jpg',
					],
				},
				{
					title: 'Ford Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-ford-car.jpg',
						'/img/img-card-landing-med-ford-truck.jpg',
					],
				},
			],
		};
	},
};
</script>

<style lang="scss">
</style>
