<template>
  <main class="featured-content" role="main">
  <section class="featured-content__showcase-card u-grid" role="region" v-for="(product, index) in products" :key="index">
    <section class="showcase-card-content__text" role="region">
      <h2 class="showcase-card-content__title" role="heading">{{product.title}}</h2>
      <p class="showcase-card-content__body">{{product.description}}</p>
      <!-- Picked a href tag here because it seems we are linking to another page -->
      <a href="#" class="showcase-card-content__button" role="link">View All</a>
    </section>
      <section class="showcase-card-content__images u-grid" role="region">
        <div class="showcase-card-content__image-container" role="region" v-for="(img, index) in product.img" :key="index">
          <a href="#" role="link">
            <div class="showcase-card-content__image-overlay" role="presentation"></div> 
              <img class="showcase-card__image--single" v-bind:src="img" v-bind:alt="product.alt[index]" role="img"/>    
              <div class="card-image__overlay-details fadein-bottom" role="contentinfo">
                <h5 class="card-image__overlay-title" role="heading">{{ product.model[index] }}</h5>
                <span class="card-image__overlay-text" role="contentinfo">Learn More</span>
              </div>
          </a>
        </div>
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
					model: ['Honda Civic', 'Honda CRV'],
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
					model: ['Audi Q7', 'Audi A6'],
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
					model: ['Chevy Camaro', 'Chevy Equionx'],
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
					model: ['Ford Mustang', 'Ford 1500'],
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
