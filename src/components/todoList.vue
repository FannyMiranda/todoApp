<template>
<div class="todoList">
    
    <todoItem v-for="(itemText,i) in todos" :todoObject="itemText" :key="i" :onRemoveTodoIndex="onRemoveTodo" :index="i"/>
   
</div>
</template>
<script>
    export default {
        name: 'todoList',
        props: ['todos', 'onRemoveTodo'],

        data() {
            return {}
        }
    }
        

</script>

<!-- add "scoped" atribute to limit css to this component only -->

<style scoped>


</style>
