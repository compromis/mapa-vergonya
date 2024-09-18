<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'es',
  },
})

useSeoMeta({
  title: 'El mapa de la vergüenza - Compromís',
  ogTitle: 'El mapa de la vergüenza - Compromís',
  description: 'Una herramienta viva donde podrás identificar cómo nos afectan de manera concreta esas políticas a lo largo del País Valenciano: puntos negros, recortes, caos, inoperancia y censura.',
  ogDescription: 'Una herramienta viva donde podrás identificar cómo nos afectan de manera concreta esas políticas a lo largo del País Valenciano: puntos negros, recortes, caos, inoperancia y censura..',
  ogImage: 'https://mapadelavergonya.com/images/ogimage.png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <main>
    <div class="container">
      <SiteHeader />
      <section class="text text-intro">
        <h1 v-motion-fade-visible class="visually-hidden">
          El mapa de la vergüenza
        </h1>

        <Languages />

        <p v-motion-fade-visible>
          Hace 500 días de las elecciones autonómicas de 2023. Unas elecciones que se tradujeron en un pacto de gobierno entre el Partido Popular y la extrema derecha.
        </p>
        <p v-motion-fade-visible>
          Un gobierno fallido, que duró un año justo. Un gobierno que ha evidenciado una gestión caótica y una hoja de ruta austericida e involucionista, enemigo del valenciano, de los servicios públicos y de los derechos y libertades logrados con Compromís en el gobierno. Un gobierno que ha empeorado todas las cifras de gestión y donde, en definitiva, la gente vive peor.
        </p>
        <p v-motion-fade-visible>
          Las consecuencias de la pésima gestión y de las políticas reaccionarias impulsadas por este gobierno fallido de la vergüenza las sufrimos de forma muy directa todas las valencianas y valencianos en el día a día de nuestros pueblos y ciudades: educación, sanidad, igualdad, políticas sociales, medio ambiente, transparencia, etc.
        </p>
        <p v-motion-fade-visible>
          Aquí tenéis el “Mapa de la vergüenza”, una herramienta viva donde podrá identificar cómo nos afectan de manera concreta esas políticas a lo largo del País Valenciano: puntos negros, recortes, caos, inoperancia y censura.
        </p>
      </section>
    </div>
    <Map />
    <Share>
      <template #title>Haz difusión</template>
      <p>Comparte esta página con tus amistades.</p>
    </Share>
  </main>
</template>
