<template>
  <div id="app" class="bg-gray-200 antialiased min-h-screen xl:flex xl:flex-col xl:h-screen">
    <site-header class="xl:flex-shrink-0"/> <!-- Site Header -->
    <div class="xl:flex-1 xl:flex xl:overflow-y-hidden">
      <search-filters />  <!-- Search & Filter section -->
      <main class="py-6 xl:flex-1 xl:overflow-x-hidden">  <!-- Main & Card section -->
        <div class="px-4">
          <h3 class="text-xl text-gray-900 font-medium">Los Angeles</h3>
          <p class="text-gray-600">Live like the stars in these luxurious Southern Califonia estates.</p>
        </div>
        <div class="mt-6 sm:overflow-x-auto">
          <div class="px-4 sm:inline-flex sm:pb-8">
            <div v-for="(property, i) in properties" :key="i" :class="{ 'mt-10 sm:ml-4': i > 1 }" class="sm:mt-0 sm:w-80 sm:flex-shrink-0">
              <property-card :property="property"/>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {
    SiteHeader: () => import('@/components/SiteHeader'),
    SearchFilters: () => import('@/components/SearchFilters'),
    PropertyCard: () => import('@/components/PropertyCard')
  },
  data () {
    return {
      properties: [
        {
          imageUrl: require('@/assets/logo.png'), // https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
          beds: 3,
          baths: 2,
          title: 'Modern home in city center',
          price: 140000,
          reviewCount: 34,
          rating: 4
        },
        {
          imageUrl: require('@/assets/logo.png'), // https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
          beds: 5,
          baths: 8,
          title: 'Modern home in city center',
          price: 290000,
          reviewCount: 24,
          rating: 6
        },
        {
          imageUrl: require('@/assets/logo.png'), // https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
          beds: 7,
          baths: 5,
          title: 'Modern home in city center',
          price: 640000,
          reviewCount: 84,
          rating: 3
        },
        {
          imageUrl: require('@/assets/logo.png'), // https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
          beds: 6,
          baths: 3,
          title: 'Modern home in city center',
          price: 960000,
          reviewCount: 34,
          rating: 4
        },
        {
          imageUrl: require('@/assets/logo.png'), // https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
          beds: 7,
          baths: 9,
          title: 'Modern home in city center',
          price: 460000,
          reviewCount: 264,
          rating: 7
        }
      ]
    }
  }
}
</script>
