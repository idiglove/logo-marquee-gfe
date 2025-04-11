<script>
	const logos = [
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/wan-nain.svg',
			alt: "Wan Nain's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/robinwood.svg',
			alt: "Robinwood's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/swapdo.svg',
			alt: "Sawpdo's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/diamond.svg',
			alt: "Diamond's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/air-car.svg',
			alt: "Air Car's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/makro-hard.svg',
			alt: "Makro hard's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/wirang.svg',
			alt: "Wirang's logo"
		},
		{
			src: 'https://vaqybtnqyonvlwtskzmv.supabase.co/storage/v1/object/public/projects-images/logo-marquee-section/starter/img/bitterfly.svg',
			alt: "Bitterfly's logo"
		}
	];

	let isPaused = false;

	const onMarqueeClick = () => {
		isPaused = !isPaused;
	};
</script>

<h1 class="py-4 text-center text-2xl">Companies</h1>

<div class="mx-auto overflow-hidden lg:max-w-[1280px]">
	<!-- svelte-ignore a11y_click_events_have_key_events -->
	<!-- svelte-ignore a11y_no_static_element_interactions -->
	<div class="flex h-16" style="width: 200%;" onclick={onMarqueeClick}>
		<div class={`animate-loop flex gap-4 ${isPaused ? 'paused' : 'playing'}`}>
			{#each logos as logo}
				<img src={logo.src} alt={logo.alt} loading="lazy" />
			{/each}
		</div>
		<div class="animate-loop flex gap-4">
			{#each logos as logo}
				<img src={logo.src} alt={logo.alt} loading="lazy" />
			{/each}
		</div>
	</div>
</div>
