<template>
  <div>
    <h1>Todoリスト</h1>
    <todo-form />
  </div>
</template>

<script>
import TodoForm from '@/components/TodoForm';
import { BadgePlugin } from 'bootstrap-vue';

export default {
  name: 'Todo',
  components: {
    TodoForm,
  },
  data() {
    return {
      todos: [],
    };
  },
  methods: {
    handleAddTodo(value) {
      if (value) {
        this.todos.push({ text: value });
      }
    },
  },
};
</script>

<style scoped>
</style>
