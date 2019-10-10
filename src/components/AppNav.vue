<template>
  <nav>
		<h3>
			Ola's Portfolio
		</h3>
		<div>
			<router-link to="/">Home</router-link>&nbsp;
    	<router-link to="/about">About</router-link>&nbsp;
			<router-link to="">Contact</router-link>
		</div>
    
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
nav {
  padding: 15px 15px;
	display: flex;
  justify-content: space-between;
	align-items: center;
}
nav a{
	margin-right: 2px;
}
</style>
