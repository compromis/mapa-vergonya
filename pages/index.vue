<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'ca',
  },
})

useSeoMeta({
  title: 'El mapa de la vergonya - Compromís',
  ogTitle: 'El mapa de la vergonya - Compromís',
  description: 'Una ferramenta viva on podreu identificar com ens afecten de manera concreta eixes polítiques al llarg del País Valencià: punts negres, retallades, caos, inoperància i censura.',
  ogDescription: 'Una ferramenta viva on podreu identificar com ens afecten de manera concreta eixes polítiques al llarg del País Valencià: punts negres, retallades, caos, inoperància i censura.',
  ogImage: 'https://mapavergonya.compromis.net/images/ogimage.png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <main>
    <div class="container">
      <SiteHeader />
      <section class="text text-intro">
        <h1 v-motion-fade-visible class="visually-hidden">
          El mapa de la vergonya
        </h1>

        <Languages />

        <p v-motion-fade-visible>
          Ara fa un any de les eleccions autonòmiques de 2023. Unes eleccions que es van traduir en un pacte de govern entre el Partit Popular i l’extrema dreta.  
        </p>
        <p v-motion-fade-visible>
          En pocs mesos, l’aliança de Carlos Mazón i els ultres en la Generalitat Valenciana ha evidenciat una gestió caòtica i un full de ruta austericida i involucionista, enemic del valencià, dels serveis públics i dels drets i llibertats assolits amb Compromís al govern. 
        </p>
        <p v-motion-fade-visible>
          Les conseqüències de la pèssima gestió i de les polítiques reaccionàries impulsades per aquest govern de la vergonya les patim de manera molt directa totes les valencianes i valencians en el dia a dia dels nostres pobles i ciutats: educació, sanitat, igualtat, polítiques socials, medi ambient, transparència, etc. 
        </p>
        <p v-motion-fade-visible>
          Ací teniu el “Mapa de la vergonya”, una ferramenta viva on podreu identificar com ens afecten de manera concreta eixes polítiques al llarg del País Valencià: punts negres, retallades, caos, inoperància i censura.
        </p>
      </section>
    </div>
    <Map />
    <Share>
      <template #title>Fes difusió!</template>
      <p>Comparteix aquesta pàgina amb les teues amistats.</p>
    </Share>
  </main>
</template>
