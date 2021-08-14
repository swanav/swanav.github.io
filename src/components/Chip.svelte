<span class="text-m px-2 font-medium {colorClass} text-white rounded-full py-0.5">
    <slot></slot>
</span>
<style>
span {
    margin: 4px 8px;
    padding: 4px 8px;
    /* display: inline; */
    justify-content: center;
    align-items: center;
    /* border-color: black;
    border-style: solid;
    border-radius: 20px; */
}
</style>

<script lang="ts">
    let classes = [
        "bg-red-500",
        "bg-purple-500",
        "bg-yellow-500",
        "bg-green-500",
        "bg-blue-500",
        "bg-indigo-500",
        "bg-pink-500"
    ];
    let colorClass = classes[Math.floor(Math.random() * classes.length)];

</script>