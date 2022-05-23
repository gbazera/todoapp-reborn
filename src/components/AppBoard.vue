<template>
	<div class="board">
        <p class="title">Board title</p>
        <p class="percent">0%</p>
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
    .board{
        cursor: pointer;
        padding: 30px;
        border-radius: 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 20px;
        border: 1px var(--light2) solid;
        color: var(--dark);
    }

    .board:hover{
        background-color: var(--light2);
    }

    .board:first-of-type{
        margin-top: 30px;
    }

    .title{
        font-size: var(--text-size);
    }

    .active{
        background-color: var(--primary);
        color: var(--light1);
        font-weight: bold;
    }
</style>