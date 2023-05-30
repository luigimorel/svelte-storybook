<script lang="ts">
	/**
	 * Kind of icon
	 * @type {'arrow-down' | 'star'  | 'arrow' | 'video'}
	 */

	export let symbol: string;

	/**
	 * @type {'light' | 'dark' }
	 */
	export let type = 'light';

	$: iconType = type === 'light' ? 'stroke-white' : 'stroke-slate-600';
</script>

{#if symbol === 'arrow-down'}
	<svg
		xmlns="http://www.w3.org/2000/svg"
		fill="none"
		viewBox="0 0 24 24"
		stroke-width="1.5"
		stroke="currentColor"
		class={`w-5 h-5 ${iconType}`}>
		<path
			stroke-linecap="round"
			stroke-linejoin="round"
			d="M9 12.75l3 3m0 0l3-3m-3 3v-7.5M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
	</svg>
{:else if symbol === 'star'}
	<svg class={`h-5 w-5 stroke-2 ${iconType}`} xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
		<path
			stroke-linecap="round"
			stroke-linejoin="round"
			d="M12.951 2.927c-.299-.92-1.602-.92-1.902 0L9.53 7.601a1 1 0 0 1-.95.69H3.664c-.968 0-1.372 1.24-.588 1.81l3.976 2.888a1 1 0 0 1 .363 1.118l-1.518 4.674c-.3.921.755 1.688 1.538 1.118l3.976-2.888a1 1 0 0 1 1.176 0l3.976 2.888c.783.57 1.838-.196 1.538-1.118l-1.518-4.674a1 1 0 0 1 .363-1.118l3.976-2.888c.783-.57.381-1.81-.588-1.81H15.42a1 1 0 0 1-.95-.69l-1.519-4.674Z" />
	</svg>
{:else if symbol === 'arrow'}
	<svg
		class={`h-5 w-5 stroke-2 ${iconType}`}
		fill="currentColor"
		viewBox="0 0 24 24"
		xmlns="http://www.w3.org/2000/svg">
		<path
			fill-rule="evenodd"
			d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
			clip-rule="evenodd" />
	</svg>
{:else if symbol === 'video'}
	<svg class={`mr-2 w-5 h-5${iconType}`} fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
		<path
			d="M2 6a2 2 0 012-2h6a2 2 0 012 2v8a2 2 0 01-2 2H4a2 2 0 01-2-2V6zM14.553 7.106A1 1 0 0014 8v4a1 1 0 00.553.894l2 1A1 1 0 0018 13V7a1 1 0 00-1.447-.894l-2 1z" />
	</svg>
{/if}
