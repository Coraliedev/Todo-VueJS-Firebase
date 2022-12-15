<template>
  <div class="todos">
    <div class="title has-text-centered">
      Todo list
    </div>
    <div class="field has-addons">
      <div class="control">
        <input class="input" type="text" placeholder="Add a todo" />
      </div>
      <div class="control">
        <a class="button is-info"> Search </a>
      </div>
    </div>
  </div>
</template>

<style>
@import "bulma/css/bulma.min.css";

.todos {
  max-width: 400px;
  padding: 20px;
  margin: 0 auto;
}
</style>
