<template>
  <main class="feature-content" role="main">
  <section class="featured-content__card u-grid" role="region" v-for="(product, index) in products" :key="index">
    <section class="card-content__text" role="region">
      <h2 class="card__title" role="heading">{{product.title}}</h2>
      <p class="card__body">{{product.description}}</p>
      <!-- Picked a href tag here because it seems we are linking to another page -->
      <a href="#" class="card__button" role="link">View All</a>
    </section>
      <section class="card-content__images u-grid" role="region">
        <section class="card-content__image-container" role="region" v-for="(img, index) in product.img" :key="index">
          <a href="#" class="card-content__image--link" role="link">
            <img class="card__image" v-bind:src="img" v-bind:alt="product.alt[index]" role="img"/>
          </a>
        </section>
      </section>    
    </section>    
  </main>
</template>

<script>
export default {
	name: 'featured-content__card',
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
					alt: ['White Honda Car', 'Red Honda SUV'],
				},
				{
					title: 'Audi Cars and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-audi-car.jpg',
						'/img/img-card-landing-med-audi-suv.jpg',
					],
					alt: ['Red Audi SUV', 'White Audi SUV'],
				},
				{
					title: 'Chevy Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-chevy-car.jpg',
						'/img/img-card-landing-med-chevy-suv.jpg',
					],
					alt: ['White Chevy Sports Car', 'Silver Chevy SUV'],
				},
				{
					title: 'Ford Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato.',
					img: [
						'/img/img-card-landing-med-ford-car.jpg',
						'/img/img-card-landing-med-ford-truck.jpg',
					],
					alt: ['White Ford Sports Car', 'Black Ford Truck'],
				},
			],
		};
	},
};
</script>

<style lang="scss">
</style>
