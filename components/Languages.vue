<template>
  <div class="d-flex toolbar">
    <ul class="languages">
      <li>
        <a href="/" :class="{ active: $route.path === '/' }">Valencià</a>
      </li>
      <li>
        <a href="/cas" :class="{ active: $route.path === '/cas' }">Castellano</a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss">
.toolbar {
  margin-top: 1.5rem;
  font-size: var(--text-sm);
}

.languages {
  list-style: none;
  display: flex;
  padding: 0;
  gap: 1rem;

  a {
    color: var(--text-muted);

    &.active {
      color: var(--white);
      font-weight: 900;
    }
  }
}

.motion {
  margin-left: auto;
  color: var(--text-muted);

  label {
    display: flex;
    gap: .5rem;
  }

  &.reduced {
    color: var(--white);
  }
}

.checkbox {
  appearance: none;
  border: 2px currentColor solid;
  border-radius: 0;
  color: currentColor;
  display: grid;
  font: inherit;
  height: 1.25em;
  margin: 0;
  place-content: center;
  width: 1.25em;

  &::before {
    content: "";
    width: 0.65em;
    height: 0.65em;
    transform: scale(0);
    transition: .25s transform ease-in-out;
    box-shadow: inset 1em 1em currentColor;
    border-radius: 100%;
  }

  &:checked::before {
    transform: scale(1);
  }

  &:focus {
    outline: 0;
    box-shadow: 0 0 0 2px var(--black);
  }
}

@include media-breakpoint-down(md) {
  .toolbar {
    flex-direction: column;
  }

  .motion {
    margin-left: 0;
    font-size: 0.9rem;
  }
}
</style>