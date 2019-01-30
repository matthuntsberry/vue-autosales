<template>
    <form class="filters u-grid" role="form">
      <select name="make" class="filters-list" role="menu">
        <optgroup label="Make" role="group">
          <option value="option1" class="filters-list__item" role="group">Make</option>
          <option value="option1" class="filters-list__item" role="group">Option 1</option>
          <option value="option2" class="filters-list__item" role="group">Option 2</option>
          <option value="option3" class="filters-list__item" role="group">Option 3</option>
          <option value="option4" class="filters-list__item" role="group">Option 4</option>
        </optgroup>
      </select>
      <select name="model" class="filters-list" role="menu">
        <optgroup label="Model">
          <option value="option1" class="filters-list__item" role="group">Model</option>
          <option value="option1" class="filters-list__item" role="group">Option 1</option>
          <option value="option2" class="filters-list__item" role="group">Option 2</option>
          <option value="option3" class="filters-list__item" role="group">Option 3</option>
          <option value="option4" class="filters-list__item" role="group">Option 4</option>
        </optgroup>
      </select>
      <select name="model" class="filters-list" role="menu">
        <optgroup label="Price">
          <option value="option1" class="filters-list__item" role="group">Price</option>
          <option value="option1" class="filters-list__item" role="group">Option 1</option>
          <option value="option2" class="filters-list__item" role="group">Option 2</option>
          <option value="option3" class="filters-list__item" role="group">Option 3</option>
          <option value="option4" class="filters-list__item" role="group">Option 4</option>
        </optgroup>
      </select>
       <input type="submit" class="filters__button" value="Find My Dream Car">
    </form>
</template>

<script>
export default {
	name: 'filters',
	data() {
		return {};
	},
};
</script>

<style lang="scss">
</style>
