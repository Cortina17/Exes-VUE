<template>
	<v-container>
		<div id="app">
			{{ message }}
		</div>

		<div>
			<input id="age" type="text" placeholder="Enter your age" />
			<button v-on:click="is-adult">Check!</button>
		</div>
		<div id="result"></div>
	</v-container>
</template>

<script>
export default {
	name: "app",
	data: () => ({
		message: "APP to tell if someone is adult after write their age",
	}),
	methods: {
		isAdult: function () {
			"result".innerHTML = "age".value >= 18 ? "Is adult" : "Is minor";
		},
	},
};
</script>
