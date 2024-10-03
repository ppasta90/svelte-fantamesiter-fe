<script>
    import "../app.css";
</script>

<div class="grid place-items-center h-screen w-full">
    <slot />
</div>

<style lang="postcss">
    :global(html) {
      background-color: theme(colors.gray.100);
    }
</style>