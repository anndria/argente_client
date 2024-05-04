<template>
    <div class="bg-white">
      <div class="mx-auto grid max-w-2xl grid-cols-1 items-center gap-x-8 gap-y-16 px-4 py-24 sm:px-6 sm:py-32 lg:max-w-7xl lg:grid-cols-2 lg:px-8">
        <div>
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Friends in College</h2>
          <p class="mt-4 text-gray-500">Plastic Edition.</p>
  
          <dl class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8">
            <div v-for="feature in features" :key="feature.name" class="border-t border-gray-200 pt-4">
              <dt class="font-medium text-gray-900">{{ feature.name }}</dt>
              <dd class="mt-2 text-sm text-gray-500">{{ feature.description }}</dd>
            </div>
          </dl>
        </div>
        <div class="grid grid-cols-2 grid-rows-2 gap-4 sm:gap-6 lg:gap-8">
          <img src="/img/1.jpg" alt="Spider Bals." class="rounded-lg bg-gray-100" />
          <img src="/img/2.jpeg" alt="Mga Plastic." class="rounded-lg bg-gray-100" />
          <img src="/img/3.jpeg" alt="Talent Search with Plastics." class="rounded-lg bg-gray-100" />
          <img src="/img/4.jpg" alt="Customer Service." class="rounded-lg bg-gray-100" />
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const features = [
    { name: 'Origin', description: 'Group form since 2021' },
    { name: 'Material', description: 'Made of Plastics, Delusion, Gaslighting, Chismis' },
    { name: 'Members', description: 'Bals, Cyril, Charls, Jobert, Haryen, Jepe, Marjo, Jeneh, Mumai' },
    { name: 'Achievements', description: 'Gastador' },
    { name: 'About', description: 'Feed them always' },
    { name: 'Favorite Traits', description: 'Drawing.' },
  ]
  </script>