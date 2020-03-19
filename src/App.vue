<template>
	<div id="app">
		<Header title="Cod3r - Base de Conhecimento" :hideToggle="false"></Header>
		<Menu></Menu>
		<Content></Content>
		<Footer></Footer>
	</div>
</template>

<script>
import Content from "./components/template/Content"
import Header from "./components/template/Header"
import Footer from "./components/template/Footer"
import Menu from "./components/template/Menu"
export default {
	name: "App",
	components: {
		Content,
		Header,
		Footer,
		Menu
	}
}
</script>

<style>
	* {
		font-family: "Lato", sans-serif;
	}

	body {
		margin: 0;
	}

	#app {
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		height: 100vh;
		display: grid;
		grid-template-rows: 60px 1fr 40px;
		grid-template-rows: 300px 1fr;
		grid-template-areas: 
			"header header" 
			"menu content" 
			"menu footer";
	}
</style>