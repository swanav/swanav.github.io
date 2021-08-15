<script lang="ts">
    export let link = "javascript:void()";
    const colors = [ "gray", "red", "yellow", "green", "blue", "indigo", "purple", "pink" ];
    const strengths = [ "300", "400", "500", "600", "700", "800", "900" ];
    const colorClass = `bg-${colors[Math.floor(Math.random() * colors.length)]}-${
        strengths[Math.floor(Math.random() * strengths.length)]
    }`;
</script>

<a href={link} target="_blank">
    <span class="text-m px-2 font-medium {colorClass} text-white rounded-full py-0.5">
        <slot />
    </span>
</a>

<style>
    span {
        margin: 4px 8px;
        padding: 4px 8px;
        justify-content: center;
        align-items: center;
    }
</style>
