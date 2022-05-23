<template>
	<nav class="container">
		<a href="#" class="logo"><span>TODO</span>APP</a>
		<ul class="nav-links">
			<li><a href="#">Log in</a></li>
			<li><a href="#" class="btn">Sign up</a></li>
		</ul>
		<button class="burger" v-on:click="toggleBoards"><i class="bx bx-menu" v-bind:class="{'bx-x': boardsToggled}"></i></button>
	</nav>
</template>

<script>
export default {
	data() {
		return {
			boardsToggled: false,
		}
	},
	methods: {
		toggleBoards(){
			this.boardsToggled = !this.boardsToggled
			const boards = document.querySelector('.boards');
			boards.classList.toggle('visible');
		}
	},
}
</script>

<style scoped>
	nav{
		background-color: var(--light1);
		height: 10vh;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	a{
		text-decoration: none;
		color: var(--dark);
		font-size: var(--text-size);
	}

	.logo{
		font-size: var(--logo-size);
		font-weight: bold;
	}

	.logo span{
		color: var(--primary);
	}

	.nav-links{
		list-style: none;
		display: flex;
		display: none;
	}

	.nav-links:last-child a{
		margin-left: 20px;
	}

	.burger{
		background-color: transparent;
		border: none;
		font-size: 28px;
		cursor: pointer;
		color: var(--dark);
		margin-top: 6px;
	}
</style>