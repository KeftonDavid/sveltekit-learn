<script lang="ts">
    let { data } = $props();
</script>

<h1 class="text-2xl font-bold">Blog</h1>

<ul>
    {#each data.summaries as {slug, title}}
        <li><a class="underline" href="/blog/{slug}">{title}</a></li>        
    {/each}
</ul>