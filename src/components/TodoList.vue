<template>
<b-container>
  <b-row :key="index" v-for="(todo, index) in todos" class="mt-2">
    <b-col cols="8" class="text-left">
      <h5>{{ todo.text }}</h5>
    </b-col>
    <b-col cols="4" class="text-right">
      <b-button>完了</b-button>
      <b-button @click="handleParentDeleteTodo(index)">削除</b-button>
    </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
  name: 'TodoList',
  props: ['todos'],
  methods: {
    handleParentDeleteTodo(index) {
      this.$emit('handleParentDeleteTodo', index);
    },
  },
};
</script>

<style scoped>

</style>
