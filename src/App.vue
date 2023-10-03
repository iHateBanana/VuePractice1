<script>
import TodoList from './components/TodoList.vue'
import Counter from './components/Counter.vue'


export default {
  components: {
    TodoList,
    Counter
  },
  data() {
    return {
      todos: ['do laundry', 'clean bathroom', 'take out trash']
    }
  }

}
</script>

<template>
  <main>
    <TodoList :todos="todos"/>
    <Counter />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
