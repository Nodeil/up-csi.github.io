<script>
    import FilterPagePanel from '$lib/components/FilterPagePanel.svelte';
    import GeneralInfo from './GeneralInfo.svelte';
    import projects from '$lib/projects/projects';
    const filters = ['All', 'Service', 'Innovation', 'Other'];
</script>

<article class="prose flex max-w-full flex-row flex-col gap-4 dark:prose-invert lg:flex-row">
    <div class="grow">
        <FilterPagePanel {filters} cardsInfo={projects} />
    </div>
    <div>
        <GeneralInfo />
    </div>
</article>
