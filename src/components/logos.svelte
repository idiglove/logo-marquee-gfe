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
</script>

<section class="animate-loop flex gap-4">
	{#each logos as logo}
		<img src={logo.src} alt={logo.alt} loading="lazy" />
	{/each}
</section>
