<script>
import Tree from "./tree.svelte";
let { items } = $props();
</script>
<ul>{#each items as item}<li>{item.name}{#if item.children.length}<Tree items={item.children} />{/if}</li>{/each}</ul>
