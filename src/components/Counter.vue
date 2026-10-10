<script setup lang="ts">
import { ref } from 'vue';

const count = ref(0);
</script>

<template>
	<div class="flex items-center gap-4 rounded-xl border border-zinc-700 bg-zinc-900 p-6">
		<button
			type="button"
			class="cursor-pointer rounded-lg bg-indigo-600 px-4 py-2 font-medium text-white transition hover:bg-indigo-500"
			@click="count--"
		>
			-
		</button>
		<span class="w-16 text-center text-3xl font-bold tabular-nums text-indigo-400">
			{{ count }}
		</span>
		<button
			type="button"
			class="cursor-pointer rounded-lg bg-indigo-600 px-4 py-2 font-medium text-white transition hover:bg-indigo-500"
			@click="count++"
		>
			+
		</button>
	</div>
</template>
