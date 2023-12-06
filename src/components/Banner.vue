<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  details: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="banner p-4">
    <h1>{{ title }}</h1>
    <h4>{{ details }}</h4>
  </div>
</template>

<style scoped>
.banner {
  background-image: url('https://via.placeholder.com/600x600');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
  color: #fff;
  text-align: center;
	height: 600px;
}

h1 {
  font-weight: 600;
  font-size: 4.3rem;
}

h4 {
	font-size: 2rem
}

@media (min-width: 768px) {
	.banner {
		margin: 0;
		width: 100%;
	}
}

@media (min-width: 1024px) {
	.banner {
		background-image: url('../assets/1920x650.png');
	}
}
</style>
