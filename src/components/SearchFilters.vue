<template>
  <section class="bg-gray-800">
    <div class="flex justify-between px-4 py-3">
      <div class="relative max-w-xs w-full">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3">
          <svg class="w-6 h-6 text-gray-600"
                stroke="currentColor" 
                xmlns:xlink="http://www.w3.org/1999/xlink" 
                xmlns="http://www.w3.org/2000/svg" 
                viewBox="0 0 24 24" 
                preserveAspectRatio="xMidYMid meet" 
                fill="none">
            <path xmlns="http://www.w3.org/2000/svg" 
                  stroke-linecap="round" 
                  stroke-linejoin="round" 
                  stroke-width="2" 
                  d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z">
            </path>
          </svg>
        </div>
        <input placeholder="Search by keywords" class="rounded-lg bg-gray-900 text-white py-2 pl-10 pr-4 focus:outline-none focus:shadow-lg focus:text-gray-900 focus:bg-white w-full">
      </div>
      <button @click="toggle = !toggle" 
              class="ml-2 inline-flex items-center pl-4 pr-3 focus:outline-none focus:shadow-outline rounded-lg shadow"
              :class="{ 'bg-gray-900': toggle, 'hover:bg-gray-600 shadow bg-gray-700': !toggle }">
        <svg class="h-6 w-6 fill-current text-gray-500" 
              viewBox="0 0 24 24" 
              xmlns="http://www.w3.org/2000/svg">
          <path d="M3 6a1 1 0 0 1 1-1h16a1 1 0 1 1 0 2H4a1 1 0 0 1-1-1zm3 6a1 1 0 0 1 1-1h10a1 1 0 1 1 0 2H7a1 1 0 0 1-1-1zm4 5a1 1 0 1 0 0 2h4a1 1 0 1 0 0-2h-4z" />
        </svg>
        <span class="ml-1 text-gray-400 font-medium">Filters</span>
      </button>
    </div>
    <form v-show="toggle">
      <div class="px-2 py-4 border-t border-gray-900 sm:flex">
        <div class="flex sm:w-1/2">
          <label class="block w-1/2 px-2">
            <span class="text-sm font-semibold text-gray-500">Bedrooms</span>
            <select class="mt-1 form-select block w-full rounded-lg bg-gray-700 text-white border-none shadow leading-snug focus:bg-gray-600">
              <option>4</option>
            </select>
          </label>
          <label class="block w-1/2 px-2">
            <span class="text-sm font-semibold text-gray-500">Bathrooms</span>
            <select class="mt-1 form-select block w-full rounded-lg bg-gray-700 text-white border-none shadow leading-snug focus:bg-gray-600">
              <option>2</option>
            </select>
          </label>
        </div>
        <div class="mt-4 sm:w-1/2 sm:mt-0">
          <label class="block px-2">
            <span class="text-sm font-semibold text-gray-500">Price Range</span>
            <select class="mt-1 form-select block w-full rounded-lg bg-gray-700 text-white border-none shadow leading-snug focus:bg-gray-600">
              <option>Up to $2,000 /wk</option>
            </select>
          </label>
        </div>
      </div>
      <div class="px-4 py-4 border-t border-gray-900">
        <span class="block text-sm font-semibold text-gray-500">Property Type</span >
        <div class="sm:flex">
          <label class="mt-3 sm:w-1/4 flex items-center">
            <input class="form-radio bg-gray-900 text-indigo-500 border-none focus:bg-gray-700" type="radio" name="propertyType" value="house">
            <span class="ml-2 text-white">House</span>
          </label>
          <label class="mt-3 sm:w-1/4 flex items-center">
            <input class="form-radio bg-gray-900 text-indigo-500 border-none focus:bg-gray-700" type="radio" name="propertyType" value="apartment">
            <span class="ml-2 text-white">Apartment</span>
          </label>
          <label class="mt-3 sm:w-1/4 flex items-center">
            <input class="form-radio bg-gray-900 text-indigo-500 border-none focus:bg-gray-700" type="radio" name="propertyType" value="loft">
            <span class="ml-2 text-white">Loft</span>
          </label>
          <label class="mt-3 sm:w-1/4 flex items-center">
            <input class="form-radio bg-gray-900 text-indigo-500 border-none focus:bg-gray-700" type="radio" name="propertyType" value="townhouse">
            <span class="ml-2 text-white">Townhouse</span>
          </label>
        </div>
      </div>
      <div class="px-4 py-4 border-t border-gray-900">
        <span class="block text-sm font-semibold text-gray-500">Amenities</span>
        <div class="sm:flex sm:-mx-2 sm:flex-wrap">
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="balcony">
            <span class="ml-2 text-white">Balcony</span>
          </label>
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="pool">
            <span class="ml-2 text-white">Pool</span>
          </label>
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="beach">
            <span class="ml-2 text-white">Beach</span>
          </label>
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="petFriendly">
            <span class="ml-2 text-white">Pet friendly</span>
          </label>
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="kidFriendly">
            <span class="ml-2 text-white">Kid friendly</span>
          </label>
          <label class="mt-3 flex items-center sm:w-1/4 sm:mx-2">
            <input class="form-checkbox bg-gray-900 text-indigo-500 border-none rounded-sm focus:bg-gray-700" type="checkbox" name="airConditioning">
            <span class="ml-2 text-white">Air Conditioning</span>
          </label>
        </div>
      </div>
      <div class="py-4 px-4 border-t border-gray-900 bg-gray-900 sm:text-right">
        <button class="block w-full sm:w-auto sm:inline-block py-2 px-2 rounded-lg text-white hover:bg-indigo-400 focus:outline-none bg-indigo-500 font-semibold focus:shadow-lg" @click.prevent>Update results</button>
      </div>
    </form>
  </section>
</template>

<script>
  export default {
    name: 'search-filters',
    data () {
      return {
        toggle: false
      }
    }
  }
</script>