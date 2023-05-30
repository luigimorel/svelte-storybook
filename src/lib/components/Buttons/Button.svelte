<script lang="ts">
	export let href: string = '';

	// Button sizes
	/**
	 * @type {'small' | 'medium' | 'large' | 'extra-large' }
	 */

	export let type: string = 'small';

	let buttonType: string;

	if (type === 'small') {
		buttonType = 'bg-slate-500 text-xs px-5 hover:bg-slate-500/90';
	} else if (type === 'medium') {
		buttonType = ' bg-red-500 px-7 text-sm hover:bg-red-500/90';
	} else if (type === 'large') {
		buttonType = ' bg-teal-500  px-9 text-base hover:bg-teal-500/90';
	} else {
		buttonType = ' bg-violet-500 text-lg px-12 hover:bg-violet-500/90';
	}
</script>

<a class={` btn ${buttonType}`} {href} target="_blank" rel="noreferrer">
	<div class="flex items-center gap-2">
		<slot />
	</div>
</a>
