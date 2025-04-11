<script>
	import Logos from '../components/logos.svelte';

	let isPaused = false;

	const onMarqueeClick = () => {
		isPaused = !isPaused;
	};
</script>

<h1 class="py-4 text-center text-2xl">Companies</h1>

<main class="mx-auto overflow-hidden lg:max-w-[1280px]">
	<!-- svelte-ignore a11y_click_events_have_key_events -->
	<!-- svelte-ignore a11y_no_static_element_interactions -->
	<div
		class={`flex h-16 ${isPaused ? 'paused' : 'playing'}`}
		style="width: 200%;"
		onclick={onMarqueeClick}
	>
		<Logos />
	</div>
</main>
