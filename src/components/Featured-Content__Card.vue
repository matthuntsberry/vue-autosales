<template>
  <main class="feature-content">
  <section class="featured-content__card u-grid" v-for="(product, index) in products" :key="index">
    <section class="card-content__text">
      <h2 class="card__title">{{product.title}}</h2>
      <p class="card__body">{{product.description}}</p>
      <a href="#" class="card__button">View All</a>
    </section>
    <section class="card-content__images">
      <a href="#">
        <picture class="card__image" v-for="(img, index) in product.img" :key="index">
          <img v-bind:src="img" />
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
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot',
					img: [
						'/img/img-card-landing-med-honda-car.jpg',
						'/img/img-card-landing-med-honda-suv.jpg',
					],
				},
				{
					title: 'Audi Cars and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot',
					img: [
						'/img/img-card-landing-med-audi-car.jpg',
						'/img/img-card-landing-med-audi-suv.jpg',
					],
				},
				{
					title: 'Chevy Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot',
					img: [
						'/img/img-card-landing-med-chevy-car.jpg',
						'/img/img-card-landing-med-chevy-suv.jpg',
					],
				},
				{
					title: 'Ford Cars, Trucks and SUVs',
					description:
						'Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot',
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
