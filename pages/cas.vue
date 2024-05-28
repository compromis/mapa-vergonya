<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'es',
  },
})

useSeoMeta({
  title: 'Escuelas en juego - Con nuestros hijos no se juega - Compromís',
  ogTitle: 'Escuelas en juego - Con nuestros hijos no se juega - Compromís',
  description: 'El gobierno de Mazón quiere que se puedan volver a dar licencias en las casas de apuestas que se encuentran junto a los centros educativos.',
  ogDescription: 'El gobierno de Mazón quiere que se puedan volver a dar licencias en las casas de apuestas que se encuentran junto a los centros educativos.',
  ogImage: 'https://escolesenjoc.comprosmis.net/images/ogimage.png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <main>
    <Hero />
    <div class="container">
      <section class="text text-intro">
        <h1 v-motion-fade-visible>
          Con nuestros<br>
          hijos e hijas<br>
          no se juega
        </h1>

        <Languages />

        <p v-motion-fade-visible>
          El gobierno de Mazón quiere que se puedan volver a dar licencias en las casas de apuestas que se encuentran junto a los centros educativos, tal y como reclama el lobby del juego.
        </p>
        <p v-motion-fade-visible>
          Esta medida supone un paso atrás en la lucha contra la ludopatía infantil y juvenil al normalizar que haya casinos o casas de juego a menos de 850 metros de institutos, centros de secundaria y de formación profesional.
        </p>
        <p>Esta es la realidad en datos:</p>
      </section>
      <section class="slot-slides">
        <div class="slot-slide">
          <SlotMachine prize="25%" id="slotMachine1">
            1 de cada 4 menores juegan en casas de apuesta de forma regular según datos del Defensor del Menor.
          </SlotMachine>
        </div>
        <div class="slot-slide">
          <SlotMachine prize="80%" id="slotMachine2">
            El 80% de las personas que sufren son menores de 30 años.
          </SlotMachine>
        </div>
        <div class="slot-slide">
          <SlotMachine prize="63%" id="slotMachine3">
            El 63% de los jóvenes menores de 25 años ha apostado en alguna ocasión.
          </SlotMachine>
        </div>
      </section>
    </div>
    <Map>
      <template #title>
        Mapa de centros educativos afectados
      </template>
      <p v-motion-fade-visible>
        Gracias al trabajo de Compromís en la Generalitat Valenciana, se logró alejar las casas de apuestas de los centros educativos.
      </p>
      <p v-motion-fade-visible>
        Ahora, con esta cesión de Mazón a la que se lucra con la ludopatía, nuestros niños y niñas podrán tener estos establecimientos en frente de la escuela al salir de clase , con el peligro que supone para este tipo de adicciones.
      </p>
      <p v-motion-fade-visible>
        En este mapa puede ver cómo está la situación:
      </p>
    </Map>
    <Share>
      <template #title>¡Difúndelo!</template>
      <p>Comparte esta página con tus amistades.</p>
    </Share>
  </main>
</template>
