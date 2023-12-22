<template>
  <div>
    <h1>Todoリスト</h1>
    <todo-form @handleParentAddTodo="handleParentAddTodo" />
    <todo-list :todos="todos"
    @handleParentDeleteTodo="handleParentDeleteTodo"/>
  </div>
</template>

<script>
import TodoForm from '@/components/TodoForm';
import TodoList from '@/components/TodoList';

export default {
  name: 'Todo',
  components: {
    TodoForm,
    TodoList,
  },
  data() {
    return {
      todos: [],
    };
  },
  methods: {
    handleParentAddTodo(value) {
      if (value) {
        this.todos.unshift({ text: value });
      }
    },
    handleParentDeleteTodo(index) {
      this.todos.splice(index, 1);
    },
  },
};
</script>

<style scoped>
</style>
