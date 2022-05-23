<template>
	<Header />
	<Main />
</template>

<script>
import Header from './components/AppHeader.vue'
import Main from './components/AppMain.vue'

export default {
	name: 'App',
	components: {
		Header,
		Main
	},
	data(){
		return{
			boards: []
		}
	}
}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		font-family: 'Poppins', sans-serif;
	}

	:root{
		--primary: #764AF1;
		--dark: #333742;
		--light1: #FFFFFF;
		--light2: #EEEEEE;
		--light-green: #4AF1B5;
		--blue: #4AA1F1;
		--red: #F14A4A;
		--logo-size: 20px;
		--heading-size: 16px;
		--text-size: 14px;
	}

	body{
		background-color: var(--light2);
		overflow-x: hidden;
	}

	.container{
		padding: 0 30px;	
	}

	.btn{
		background-color: var(--primary);
		color: var(--light1) !important;
		padding: 10px 15px;
		font-weight: bold;
		border-radius: 10px;
		border: none;
	}

	.heading{
		color: var(--dark);
		font-weight: bold;
		font-size: var(--heading-size);
	}
</style>