<!-- app/app.vue -->
<template>
  <UApp>
    <div
      class="min-h-screen bg-gray-50 dark:bg-gray-950 text-gray-900 dark:text-gray-100 flex flex-col justify-between">
      <!-- Navbar -->
      <header
        class="border-b border-gray-200 dark:border-gray-800 bg-white/80 dark:bg-gray-900/80 backdrop-blur sticky top-0 z-50">
        <UContainer class="flex items-center justify-between h-16">
          <NuxtLink to="/" class="font-bold text-lg tracking-tight hover:opacity-80 transition">
            MiPortafolio<span class="text-primary-500">.dev</span>
          </NuxtLink>

          <nav class="flex items-center gap-6 text-sm font-medium">
            <NuxtLink to="/" class="hover:text-primary-500 transition">Inicio</NuxtLink>
            <NuxtLink to="/proyectos" class="hover:text-primary-500 transition">Proyectos</NuxtLink>

            <ClientOnly>
              <UButton :icon="$colorMode.value === 'dark' ? 'i-heroicons-moon-20-solid' : 'i-heroicons-sun-20-solid'"
                color="neutral" variant="ghost" aria-label="Theme"
                @click="$colorMode.preference = $colorMode.value === 'dark' ? 'light' : 'dark'" />
            </ClientOnly>
          </nav>
        </UContainer>
      </header>

      <!-- Contenido Dinámico -->
      <main class="grow">
        <NuxtPage />
      </main>

      <!-- Footer -->
      <footer class="border-t border-gray-200 dark:border-gray-800 py-6 text-center text-xs text-neutral-500">
        <p>© {{ new Date().getFullYear() }} - Portafolio & Servicios Freelance</p>
      </footer>
    </div>
  </UApp>
</template>