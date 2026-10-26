<script>
let { n } = $props();
let id = $props.id();
</script>
<div id={id}>{#if n === 1}<p>one</p>{:else if n === 2}<p>two</p>{:else}<p>other</p>{/if}{#each [1, 2] as i}<i>{i}</i>{/each}</div>
