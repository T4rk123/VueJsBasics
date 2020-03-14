<template>
  <div id="app">
    <h1>Vue js app</h1> 
    <ToDoList
      v-bind:todos="todos"
    />
  </div>
</template>

<script>
import ToDoList from '@/components/ToDoList'
export default {
  name: 'app',
  data (){
    return {
      todos: [
        {id: 1, title: 'Установить VS Code', completed: false, imagesourse:"https://bipbap.ru/wp-content/uploads/2017/08/2.jpg"},
        {id: 2, title: 'Сделать fork https://github.com/grishinrv/VueJsBasics', completed: false,imagesourse:"https://klike.net/uploads/posts/2018-06/1528720172_1.jpg"},
        {id: 3, title: 'Разработать просто приложение-список', completed: false,imagesourse:"https://www.cruzo.net/user/images/k/ecc3ecf42c75db1ffce5d06cbe95b1e6_644.jpg"}
      ]
    }
  },
  components: {
    ToDoList
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
