<script lang="ts">
    export let url: string;
</script>

<a href={url} target="_blank"><slot /></a>

<style>
    a:hover {
        color: #00B2FF;
    }
    a {
        color: #333333;
        font-weight: 300;
    }
</style>