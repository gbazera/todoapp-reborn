<template>
	<div class="boards">
        <div class="top">
            <p class="heading">Your boards</p>
            <a class="add-board"><i class="bx bx-plus"></i></a>
        </div>
        <div class="items">
            <Board />
        </div>
    </div>
</template>

<script>
import Board from './AppBoard.vue'

export default {
    components:{
        Board
    },
	data() {
		return {
		
		}
	}
}
</script>

<style scoped>
    .boards{
        width: 100%;
        position: absolute;
        background-color: var(--light1);
        left: 100%;
        top: 10vh;
        height: 90vh;
        padding: 0 30px;
        transition: left .2s;
    }

    .visible{
        left: 0;
    }

	.top{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .add-board{
        color: var(--primary);
        font-size: var(--logo-size);
        cursor: pointer;
    }
</style>