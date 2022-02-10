<template>
	<v-container>
		<div id="app">
			{{ message }}
		</div>
		<v-footer dark padless>
			<v-card class="flex" flat tile>
				<v-card-title class="teal">
					<strong class="subheading"
						>Get connected with us on social networks!</strong
					>
					<v-spacer></v-spacer>
				</v-card-title>

				<v-card-text class="py-2 white--text text-center">
					{{ new Date().getFullYear() }} — <strong>Vuetify</strong>
				</v-card-text>
			</v-card>
		</v-footer>
	</v-container>
</template>

<script>
export default {
	name: "app",
	data: () => ({
		message: "APP to tell if someone is adult after write their age",
	}),
};
</script>
