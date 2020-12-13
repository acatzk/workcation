<template>
  <div id="app" class="bg-gray-200 antialiased min-h-screen">
    <!-- Header section -->
    <header class="flex items-center justify-between bg-gray-900 px-4 py-3">
      <svg class="h-8 w-auto" 
           viewBox="0 0 185 32" 
           fill="none" 
           xmlns="http://www.w3.org/2000/svg">
        <path d="M121.09 28.336c2.352 0 4.392-1.248 5.424-3.12l-2.688-1.536c-.48.984-1.512 1.584-2.76 1.584-1.848 0-3.216-1.368-3.216-3.264 0-1.92 1.368-3.288 3.216-3.288 1.224 0 2.256.624 2.736 1.608l2.664-1.56c-.984-1.848-3.024-3.096-5.376-3.096-3.648 0-6.336 2.76-6.336 6.336 0 3.576 2.688 6.336 6.336 6.336zM137.084 16v1.416c-.864-1.08-2.16-1.752-3.912-1.752-3.192 0-5.832 2.76-5.832 6.336 0 3.576 2.64 6.336 5.832 6.336 1.752 0 3.048-.672 3.912-1.752V28h3.096V16h-3.096zm-3.336 9.384c-1.896 0-3.312-1.368-3.312-3.384s1.416-3.384 3.312-3.384c1.92 0 3.336 1.368 3.336 3.384s-1.416 3.384-3.336 3.384zM149.851 18.976V16h-2.712v-3.36l-3.096.936V16h-2.088v2.976h2.088v4.992c0 3.24 1.464 4.512 5.808 4.032v-2.808c-1.776.096-2.712.072-2.712-1.224v-4.992h2.712zM153.57 14.56c1.056 0 1.92-.864 1.92-1.896s-.864-1.92-1.92-1.92c-1.032 0-1.896.888-1.896 1.92s.864 1.896 1.896 1.896zM152.034 28h3.096V16h-3.096v12zM163.676 28.336c3.528 0 6.36-2.76 6.36-6.336 0-3.576-2.832-6.336-6.36-6.336-3.528 0-6.336 2.76-6.336 6.336 0 3.576 2.808 6.336 6.336 6.336zm0-3.024c-1.824 0-3.24-1.368-3.24-3.312 0-1.944 1.416-3.312 3.24-3.312 1.848 0 3.264 1.368 3.264 3.312 0 1.944-1.416 3.312-3.264 3.312zM178.886 15.664c-1.608 0-2.856.6-3.576 1.68V16h-3.096v12h3.096v-6.48c0-2.088 1.128-2.976 2.64-2.976 1.392 0 2.376.84 2.376 2.472V28h3.096v-7.368c0-3.192-1.992-4.968-4.536-4.968z"       
              fill="#A3BFFA"/>
        <path d="M61.063 28h3.768l3.144-11.088L71.143 28h3.768l4.704-16.8h-3.48L72.92 23.656 69.391 11.2H66.56l-3.504 12.456L59.84 11.2h-3.48L61.063 28zM85.674 28.336c3.528 0 6.36-2.76 6.36-6.336 0-3.576-2.832-6.336-6.36-6.336-3.528 0-6.336 2.76-6.336 6.336 0 3.576 2.808 6.336 6.336 6.336zm0-3.024c-1.824 0-3.24-1.368-3.24-3.312 0-1.944 1.416-3.312 3.24-3.312 1.848 0 3.264 1.368 3.264 3.312 0 1.944-1.416 3.312-3.264 3.312zM97.308 18.064V16h-3.096v12h3.096v-5.736c0-2.52 2.04-3.24 3.648-3.048V15.76c-1.512 0-3.024.672-3.648 2.304zM113.831 28l-4.968-6.072L113.687 16h-3.696l-4.128 5.28V11.2h-3.096V28h3.096v-5.448L110.231 28h3.6z" 
              fill="#fff"/>
        <path fill-rule="evenodd" 
              clip-rule="evenodd" 
              d="M43.911 12.604L36.213 8.16v20.645h9v2h-44v-2h4v-12.72l-3.728.933L1 15.078l21.09-5.273h3.122a9.552 9.552 0 0 0-.68 2.559l-.483 3.975 5.164-2.982v15.448h5V8.161l-7.696 4.444a7.502 7.502 0 0 1 2.565-4.8h-4.12a7.489 7.489 0 0 1 6.646-2.973l-5.591-3.228a7.488 7.488 0 0 1 6.696.402c1.039.6 1.88 1.41 2.5 2.347a7.461 7.461 0 0 1 2.5-2.347 7.49 7.49 0 0 1 6.698-.402l-5.593 3.228a7.488 7.488 0 0 1 6.646 2.973h-4.12a7.498 7.498 0 0 1 2.567 4.8zM25.213 28.805v-10h-6v10h6zm-11-8a2 2 0 1 1-4 0 2 2 0 0 1 4 0z" 
              fill="#A3BFFA"/>
      </svg>
      <button class="focus:outline-none">
        <svg stroke="currentColor"  
             class="w-6 h-6 text-gray-500"
             xmlns:xlink="http://www.w3.org/1999/xlink" 
             xmlns="http://www.w3.org/2000/svg" 
             viewBox="0 0 24 24" 
             preserveAspectRatio="xMidYMid meet" 
             fill="none">
          <path xmlns="http://www.w3.org/2000/svg" 
                stroke-linecap="round" 
                stroke-linejoin="round" 
                stroke-width="2" 
                d="M4 6h16M4 12h8m-8 6h16">
          </path>
        </svg>
      </button>
    </header>
    <!-- Filter section -->
    <section class="flex justify-between bg-gray-800 px-4 py-3">
      <div class="relative">
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
        <input placeholder="Search by keywords" class="rounded-lg bg-gray-900 text-white py-2 pl-10 pr-4 focus:outline-none focus:shadow-lg focus:text-gray-900 focus:bg-white">
      </div>
      <button class="inline-flex items-center hover:bg-gray-600 pl-4 pr-3 focus:outline-none focus:shadow-outline rounded-lg bg-gray-700 shadow">
        <svg class="h-6 w-6 fill-current text-gray-500" 
              viewBox="0 0 24 24" 
              xmlns="http://www.w3.org/2000/svg">
          <path d="M3 6a1 1 0 0 1 1-1h16a1 1 0 1 1 0 2H4a1 1 0 0 1-1-1zm3 6a1 1 0 0 1 1-1h10a1 1 0 1 1 0 2H7a1 1 0 0 1-1-1zm4 5a1 1 0 1 0 0 2h4a1 1 0 1 0 0-2h-4z" />
        </svg>
        <span class="ml-1 text-gray-400 font-medium">Filters</span>
      </button>
    </section>
    <!-- main section -->
    <main class="px-4 py-6">
      <h3 class="text-xl text-gray-900 font-medium">Los Angeles</h3>
      <p class="text-gray-600">Live like the stars in these luxurious Southern Califonia estates.</p>
      <div class="mt-6">
        <div>
          <div>
            <img class="rounded-lg shadow-md h-64" 
               src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" 
               alt="house-image">
          </div>
          <div class="relative px-4 -mt-16">
            <div class="bg-white px-4 py-4 rounded-lg shadow-lg">
              <div class="flex">
                <span class="bg-green-200 text-green-800 font-semibold rounded-full px-2 py-1 leading-none inline-block text-xs uppercase tracking-wide">Plus</span>
                <div class="ml-2 text-sm text-gray-600 font-semibold tracking-wide uppercase">
                  3 Beds &bull; 2 baths
                </div>
              </div>
              <h4 class="mt-1 text-lg text-gray-900 font-semibold">Modern home in city center</h4>
              <div class="mt-1">
                <span class="text-gray-900">$1,400</span>
                <span class="ml-1 text-sm text-gray-600">/wk</span>
              </div>
              <div class="mt-2 text-sm text-gray-600 flex items-center">
                <svg v-for="i in 5" :key="i" 
                     class="h-4 w-4 fill-current text-green-400"
                     viewBox="0 0 24 24" 
                     xmlns="http://www.w3.org/2000/svg">
                  <path d="M8.128 19.825a1.586 1.586 0 0 1-1.643-.117 1.543 1.543 0 0 1-.53-.662 1.515 1.515 0 0 1-.096-.837l.736-4.247-3.13-3a1.514 1.514 0 0 1-.39-1.569c.09-.271.254-.513.475-.698.22-.185.49-.306.776-.35L8.66 7.73l1.925-3.862c.128-.26.328-.48.577-.633a1.584 1.584 0 0 1 1.662 0c.25.153.45.373.577.633l1.925 3.847 4.334.615c.29.042.562.162.785.348.224.186.39.43.48.704a1.514 1.514 0 0 1-.404 1.58l-3.13 3 .736 4.247c.047.282.014.572-.096.837-.111.265-.294.494-.53.662a1.582 1.582 0 0 1-1.643.117l-3.865-2-3.865 2z"/>
                </svg>
                <span class="ml-2">34 reviews</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>
