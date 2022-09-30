<template>
  <div class="mx-auto">
    <div class="text-center">
      <Heading1>Just another todo app</Heading1>
    </div>
    <div class="shadow-lg mt-8 max-w-lg mx-auto">
      <TodoItem v-for="todo in todos" :todo="todo"/>
      <TodoCreate />
    </div>
  </div>
</template>
<script setup>
import Heading1 from "../typography/Heading1.vue";
import TodoItem from "../todo/TodoItem.vue";
import TodoCreate from "../todo/TodoCreate.vue";
import {ref} from "vue";

const todos = ref([
  { body: 'Hello there', completed: false,},
  { body: 'Hello there', completed: false,},
  { body: 'Hello there', completed: false,},
  { body: 'Hello there', completed: false,},
  { body: 'Hello there', completed: false,},
  { body: 'Hello there', completed: false,},
])

</script>