<template>
  <section class="map">
    <iframe
          src="https://www.google.com/maps/d/embed?mid=1SZDlQAEBkjJstr56Goomo9HscZB4fS0&ehbc=2E312F"
          width="640"
          height="680"
          class="map-embed" />
  </section>
</template>

<style lang="scss" scoped>
iframe {
  display: block;
  width: 100%;
  margin-top: -5rem;
}

.map {
  padding: var(--site-padding);
  border-radius: 1rem;
  overflow: hidden;
  max-width: 1300px; 
  margin: 0 auto;
}
</style>