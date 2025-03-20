<script lang="ts">
    import { counter } from "./counter.svelte";

    let localCount = $state(0);
</script>

<h1>Main page</h1>
<a href="/test">Test page</a>

<br />
<br />

<button
    onclick={() => {
        counter.count += 1;
        localCount += 1;
    }}>+1</button
>
<p>Global count: {counter.count}</p>
<p>Local count: {localCount}</p>
