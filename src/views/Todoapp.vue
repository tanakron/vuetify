<template>
  <v-container>
    <v-row
      class="d-flex flex-row align-center ma-10"
      v-for="(item, index) in todos"
      :key="index"
    >
      <v-checkbox v-model="value" value="value"></v-checkbox>
      <span>Title</span>
      <span>{{ item.title }}</span>
      <br />
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        { id: 2, title: "Task23", completed: true },
        { id: 3, title: "Task33", completed: false },
        { id: 1, title: "Task13", completed: true },
      ],
    };
  },
};
</script>

<style></style>
