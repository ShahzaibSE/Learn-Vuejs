<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <router-view/> -->
     <todo-list v-bind:todos="todos"></todo-list>
     <!-- <HelloWorld></HelloWorld> -->
  </div>
</template>

<script>
import TodoList from './components/TodoList'
// import HelloWorld from '@/components/HelloWorld'
export default {
  name: 'app',
  components: {
    TodoList
  },
  data () {
    return {
      todos: [
        {
          title: 'A',
          project: 'Project A',
          done: false
        },
        {
          title: 'B',
          project: 'Project B',
          done: false
        },
        {
          title: 'C',
          project: 'Project C',
          done: false
        },
        {
          title: 'D',
          project: 'Project D',
          done: false
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
