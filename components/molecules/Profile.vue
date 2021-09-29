<template>
	<div class="flex items-center">
		<img
			class="mr-6 w-20 h-20 rounded-full object-cover"
			src="https://fashionsista.co/wallpaper/wallpaper/20210227/hot-anime-guys-book-1-oreki-houtarou-wattpad-preview.jpg"
			alt="Avatar"
		/>

		<div class="flex flex-col w-full">
			<strong class="text-title text-2xl">Thiago Silva</strong>
			<p class="flex items-center">
				<img src="icons/level.svg" alt="level" class="mr-2" />
				<span class="text-base">Level {{ level }}</span>
			</p>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import { mapState } from 'vuex';

export default Vue.extend({
	computed: mapState('Challenges', ['level']),
});
</script>
