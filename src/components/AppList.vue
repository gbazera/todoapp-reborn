<template>
	<div class="list">
        <div class="top">
            <p class="heading">Todo list</p>
            <a class="add-todo"><i class="bx bx-plus"></i></a>
        </div>
        <div class="todos">
            <Todo />
        </div>
    </div>
</template>

<script>
import Todo from './AppTodo.vue'

export default {
    components:{
        Todo
    },
	data() {
		return {
		
		}
	}
}
</script>

<style scoped>
    .list{
        width: 100%;
    }

	.top{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .add-todo{
        color: var(--primary);
        font-size: var(--logo-size);
        cursor: pointer;
    }
</style>