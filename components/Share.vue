<template>
  <section class="share">
    <div class="outline-card">
      <div class="header">
        <div class="header-content">
          <h2><slot name="title" /></h2>
          <div class="text">
            <slot />
          </div>
        </div>
      </div>
      <div class="share-links">
        <a href="whatsapp://send?text=https://mapavergonya.compromis.net" class="link whatsapp">
          <span>-&gt;</span> WhatsApp
        </a>
        <a href="https://t.me/share/url?url=https://mapavergonya.compromis.net&text=" class="link telegram">
          <span>-&gt;</span> Telegram
        </a>
        <a href="https://www.facebook.com/sharer/sharer.php?u=https://mapavergonya.compromis.net" class="link facebook">
          <span>-&gt;</span> Facebook
        </a>
        <a href="https://twitter.com/intent/tweet/?text=&url=https://mapavergonya.compromis.net&hashtags=SalvemEscoles" class="link twitter">
          <span>-&gt;</span> X / Twitter
        </a>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.share {
  margin: 6rem 0;

  .outline-card {
    max-width: var(--text-container);
    border: 2px var(--white) solid;
    border-radius: 1rem;
    margin: 0 auto;
    position: relative;

    .header {
      position: relative;
      display: flex;
      gap: 1rem;

      &-content {
        padding: 1.5rem;
      }
    }

    h2 {
      padding-bottom: 0;
      margin-bottom: .5rem;
    }

    .text :deep(p) {
      margin: 1rem 0 0 !important;
      font-size: var(--text-md);
    }

    .link {
      display: flex;
      border-top: 2px var(--white) solid;
      color: var(--white);
      padding: 1.5rem;
      font-size: var(--text-lg);
      transition: .25s ease;
      align-items: center;

      &:nth-child(odd) {
        border-right: 2px var(--white) solid;
      }

      &:hover {
        background: var(--white);
        color: var(--primary);
        text-decoration: none;

        span {
          width: 1.25em;
          transform: translateX(0);
        }
      }

      span {
        display: block;
        width: 0;
        overflow: hidden;
        transition: .5s ease;
        white-space: nowrap;
        transform: translateX(-100%);
      }
    }
  }

  &-links {
    display: grid;
    grid-template-columns: 1fr 1fr;

    .facebook {
      border-radius: 0 0 0 .85rem;
    }

    .twitter {
      border-radius: 0 0 .85rem 0;
    }
  }
}

@include media-breakpoint-down(md) {
  .share {
    .header {
      flex-direction: column;
    }
  }
}
</style>