<template>
	<div>
		<li>
			{{todo.text}}
			<button @click="$emit('remove', todo.id)">
			 X
			</button>
		</li>
	</div>
</template>
<script>
	export default {
		props: {
			todo: {
				type: Object,
				required: true
			}
		}

	}
</script>
<style>
	
</style>