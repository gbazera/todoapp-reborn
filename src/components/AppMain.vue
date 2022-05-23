<template>
	<main class="container">
        <List />
		<Boards />
    </main>
</template>

<script>
import List from './AppList.vue'
import Boards from './AppBoards.vue'

export default {
    components: {
		List,
		Boards
	},
	data() {
		return {
		
		}
	}
}
</script>

<style scoped>
	main{
        margin-top: 30px;
        display: flex;
        justify-content: space-between;
    }
</style>