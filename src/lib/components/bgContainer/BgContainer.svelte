<script>
	import BlurEffect from './BgCard.png';
</script>

<div class="parent d-flex align-items-center justify-content-center text-white rounded">
	<div
		class="position-relative overflow-hidden   m-4 rounded-4 container d-flex flex-column align-items-center justify-content-center "
		style="padding:36px 60px 24px 60px; border: 1px solid var(--bg-container-border); max-width: 420px;"
	>
		<div
			style="position:absolute; top:0;
    left:0; right:0; bottom:0;"
		>
			<img class="position-absolute" src={BlurEffect} alt="" style="width: 100%; height:100%; " />
		</div>

		<div
			class=" d-flex flex-column align-items-center justify-content-center w-100"
			style="z-index: 100;"
		>
			<slot />
		</div>
	</div>
</div>

<style>
	.parent {
		min-height: 100vh;
		overflow: auto;
	}
</style>
