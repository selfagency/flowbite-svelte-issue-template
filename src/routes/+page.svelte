<script>
  import { Badge, Indicator, Select, Heading, P, List, Li, Label, MultiSelect } from 'flowbite-svelte';

  let color = 'green';


</script>

<div class='p-9'>

<Label for "color">Color</Label>
<Select name="color" items={[{ name: 'Green', value: 'green' }, { name: 'Red', value: 'red' }]} on:change={e => (color = e.target.value)} />

<Badge {color}>Test Badge</Badge>

<Indicator {color} />

</div>

