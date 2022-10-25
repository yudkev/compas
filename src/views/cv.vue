<template>
  <div class="about">
    <h1>This is an third page</h1>
    <div class="columns">
      <div class="column">
        First column
      </div>
      <div class="column">
        Second column
      </div>
      <div class="column">
        Third column
      </div>
      <div class="column">
        <div class="buttons">
          <button class="button is-info" >Info</button>
          <RouterLink to="/about">
            <button class="button is-success">About</button>
          </RouterLink>
          <button class="button is-warning">Warning</button>
          <button class="button is-danger">Danger</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
