<template>
  <div class="todos">
    <div class="title has-text-centered">Todo list</div>
    <div class="field is-grouped mb-5">
      <p class="control is-expanded">
        <input class="input" type="text" placeholder="Add todo" />
      </p>
      <p class="control">
        <a class="button is-info"> Add </a>
      </p>
    </div>
    <div v-for="todo in todos" :key="todo.id" class="card mb-5">
      <div class="card-content">
        <div class="content">
          <div class="columns is-mobile is-vcentered">
            <div class="column">{{todo.content}}</div>
            <div class="column is-5 has-text-right">
              <button class="button is-light">&check;</button>
              <button class="button is-danger ml-2">&cross;</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
/* imports */
import { ref } from "vue";

/* todos */
const todos = ref([
  { id: "id1", content: "todo1", done: false },
  { id: "id2", content: "todo2", done: false },
]);

</script>

<style>
@import "bulma/css/bulma.min.css";

.todos {
  max-width: 400px;
  padding: 20px;
  margin: 0 auto;
}
</style>
