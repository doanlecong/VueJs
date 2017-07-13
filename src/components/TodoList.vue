<template>
  <div class="container">
    
    <p class="text-success"><strong>Completed Tasks :{{todos.filter(todo =>{return todo.done === true}).length}}</strong></p>
    <p class="text-warning">Pending Tasks : {{todos.filter(todo => {return todo.done === false}).length}}</p>
    <ul class="list-group">
        <li class="list-group-item">Item 1</li>
        <li class="list-group-item">Item 2</li>
        <li class="list-group-item">Item 3</li>
    </ul>
    <div class="container">
        <todo v-for="todo in todos" v-bind="todo"></todo>
    </div>
  </div>
</template>
<script type="text/javascript">
    import Todo from './Todo'
    export default {
        name: 'todolist',
        props:['todos'],
        components:{
            Todo,
        }
    }
</script>
<style>

</style>
