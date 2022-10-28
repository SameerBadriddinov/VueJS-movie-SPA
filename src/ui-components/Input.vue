<template>
	<input type="text" class="form-control" :value="modelValue" @input="updateInput" />
</template>

<script>
export default {
	name: 'Input',
	props: {
		modelValue: [String, Number],
		term: [String, Number],
	},
	methods: {
		updateInput(e) {
			this.$emit('update:modelValue', e.target.value)
		},
	},
}
</script>

<style></style>
