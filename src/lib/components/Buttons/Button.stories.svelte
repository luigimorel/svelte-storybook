<script lang="ts">
	import { Meta, Story } from '@storybook/addon-svelte-csf';

	import Button from './Button.svelte';
</script>

<Meta title="Buttons" component={Button} />

<!-- Small -->
<Story name="Small">
	<Button href="https://google.com">Small Button</Button>
</Story>

<!-- medium -->
<Story name="Medium">
	<Button type="medium" href="https://google.com">Medium Button</Button>
</Story>

<!-- large-->
<Story name="Large">
	<Button type="large" href="https://google.com">Large Button</Button>
</Story>

<!-- extra-large-->
<Story name="Extra Large">
	<Button type="extra-large" href="https://google.com">Extra Large Button</Button>
</Story>
