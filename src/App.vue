<script setup>
  import MainContent from './components/MainContent.vue';
</script>

<template>
  <div id="body-wrap">
		<div class="container">

			<header id="header">
				<div class="logo">
          1PercentDesignHub
          <!-- <img src="./components/img/logo.png" alt=""> -->
				</div>	
			</header>
      <MainContent/>
		</div>
	</div><!--body-wrap-->
</template>

<style scoped>
  .logo{
    font-family: 'Roboto';
    font-style: italic;
    font-size: 2.2rem;
    font-weight: 100;
  }
</style>

