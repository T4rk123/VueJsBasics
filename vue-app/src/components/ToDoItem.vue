<template>
    <li>
        <span>
            <input type="checkbox">
            <strong>{{todo.id}}</strong>
            {{todo.title}}
        </span>
        <img :src="todo.imagesourse"/>
    </li>
</template>

<script>
export default {
    props: {
        todo:{
            type: Object,
            required: true
        }
    }
}
</script>