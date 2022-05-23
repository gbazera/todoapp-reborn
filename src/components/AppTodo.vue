<template>
	<div class="todo">
        <p class="title">Todo title</p>
        <div class="buttons">
            <a class="check"><i class="bx bx-check"></i></a>
            <a class="edit"><i class="bx bx-edit-alt"></i></a>
            <a class="remove"><i class="bx bx-trash"></i></a>
        </div>
    </div>
</template>

<script>
export default {
	data() {
		return {
		
		}
	}
}
</script>

<style scoped>
    .todo{
        padding: 30px;
        background-color: var(--light1);
        border-radius: 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 20px;
    }

    .todo:first-of-type{
        margin-top: 30px;
    }

    .title{
        color: var(--dark);
        font-size: var(--text-size);
    }

    .buttons a{
        margin-left: 10px;
        font-size: var(--logo-size);
        cursor: pointer;
    }

    .check{
        color: var(--light-green);
    }

    .edit{
        color: var(--blue);
    }

    .remove{
        color: var(--red);
    }

    .completed{
        background-color: var(--light-green);
    }

    .completed a{
        color: var(--dark);
    }

    .completed p{
        text-decoration: line-through;
    }
</style>