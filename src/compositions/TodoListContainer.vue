<template></template>

<srcript>
    import { ref, readonly, provide } from 'vue'
    export default {
        name: 'TodoListContainer',
        setup() {
            const todos = ref([])
            provide('todos', readonly(tools))
            const initTodos = (init_todos) => [
                todos.value = init_todos
            ]
            const addTodo = (todo, date) => {}
            const removeTodo = (id) => {}
            const completeTodo= (id) => {}

            provide('addTodo', addTodo)
            provide('removeTodo', removeTodo)
            provide('completeTodo', completeTodo)
        },
    }
</srcript>