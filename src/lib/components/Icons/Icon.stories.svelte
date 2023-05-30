<script>
	import { Meta, Story } from '@storybook/addon-svelte-csf';

	import Icon from './Icon.svelte';
</script>

<Meta title="Icons" component={Icon} />

<!-- Light -->
<Story name="Arrow Down - Light">
	<Icon symbol="arrow-down" />
</Story>

<Story name="Arrow - Dark">
	<Icon type="dark" symbol="arrow" />
</Story>

<Story name="Arrow Down - Dark">
	<Icon type="dark" symbol="arrow-down" />
</Story>

<Story name="Star - Dark">
	<Icon type="dark" symbol="star" />
</Story>

<Story name="Video - Dark">
	<Icon type="dark" symbol="video" />
</Story>
