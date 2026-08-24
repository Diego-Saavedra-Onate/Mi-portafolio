<!-- app/pages/index.vue -->
<template>
    <UContainer class="py-16 space-y-16">
        <!-- Hero Section -->
        <section class="text-center max-w-2xl mx-auto space-y-4">
            <UBadge color="primary" variant="subtle" size="md">Disponible para proyectos freelance</UBadge>

            <h1 class="text-4xl sm:text-5xl font-extrabold tracking-tight">
                Soluciones Web, Scripts en Python y Datos
            </h1>

            <p class="text-gray-600 dark:text-gray-400 text-base sm:text-lg">
                Desarrollo páginas web rápidas para pymes, scripts de automatización/scraping y extracción de reportes
                SQL a medida.
            </p>

            <div class="flex justify-center gap-4 pt-2">
                <UButton to="https://wa.me/56962019028" target="_blank" icon="i-heroicons-chat-bubble-left-right"
                    size="lg" color="primary">
                    Contactar por WhatsApp
                </UButton>
                <UButton to="/proyectos" variant="outline" size="lg" color="neutral">
                    Ver proyectos
                </UButton>
            </div>
        </section>

        <!-- Sección de Servicios -->
        <section class="space-y-6">
            <div class="text-center">
                <h2 class="text-2xl font-bold">Servicios que ofrezco</h2>
                <p class="text-gray-500 text-sm">Trabajos rápidos, transparentes y a precio accesible.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <UCard>
                    <template #header>
                        <div class="flex items-center gap-2">
                            <UIcon name="i-heroicons-globe-alt" class="w-6 h-6 text-primary-500" />
                            <h3 class="font-semibold">Landing Pages</h3>
                        </div>
                    </template>
                    <p class="text-sm text-gray-500 dark:text-gray-400">
                        Sitios web modernos, responsivos para celulares y optimizados para negocios locales o
                        profesionales independientes.
                    </p>
                </UCard>

                <UCard>
                    <template #header>
                        <div class="flex items-center gap-2">
                            <UIcon name="i-heroicons-command-line" class="w-6 h-6 text-primary-500" />
                            <h3 class="font-semibold">Automatización Python</h3>
                        </div>
                    </template>
                    <p class="text-sm text-gray-500 dark:text-gray-400">
                        Extracción web (scraping), limpieza y cruce de datos masivos en Excel/CSV y scripts a medida.
                    </p>
                </UCard>

                <UCard>
                    <template #header>
                        <div class="flex items-center gap-2">
                            <UIcon name="i-heroicons-circle-stack" class="w-6 h-6 text-primary-500" />
                            <h3 class="font-semibold">Bases de Datos & SQL</h3>
                        </div>
                    </template>
                    <p class="text-sm text-gray-500 dark:text-gray-400">
                        Creación de esquemas relacionales, consultas complejas, reportes y optimización de datos.
                    </p>
                </UCard>
            </div>
        </section>
    </UContainer>
</template>