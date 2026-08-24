<!-- app/pages/proyectos/scraping.vue -->
<template>
    <UContainer class="py-12 max-w-3xl space-y-6">
        <UButton to="/proyectos" variant="ghost" color="neutral" icon="i-heroicons-arrow-left">
            Volver a proyectos
        </UButton>

        <header class="space-y-2">
            <div class="flex items-center gap-2">
                <UBadge color="primary">Python</UBadge>
                <UBadge color="neutral">Pandas</UBadge>
            </div>
            <h1 class="text-3xl font-bold">Extracción y Limpieza Masiva de Datos</h1>
        </header>

        <div class="prose dark:prose-invert max-w-none text-gray-600 dark:text-gray-300 space-y-4">
            <p>
                Este proyecto automatiza la descarga de listados de precios desde sitios web públicos para comparar
                variaciones mensuales sin intervención manual.
            </p>

            <h3 class="text-lg font-bold text-gray-900 dark:text-gray-100">Características:</h3>
            <ul class="list-disc pl-5 space-y-1 text-sm">
                <li>Extracción periódica mediante <code>BeautifulSoup</code>.</li>
                <li>Eliminación de duplicados y formateo de moneda con <code>pandas</code>.</li>
                <li>Generación de un archivo <code>.xlsx</code> listo para reportes ejecutivos.</li>
            </ul>
        </div>
    </UContainer>
</template>