<script lang="ts">
    import Chip from "./components/Chip.svelte";
    import Heading from "./components/Heading.svelte";

    const skills = [
        {
            name: "C",
            url: "https://en.wikipedia.org/wiki/C_(programming_language)",
        },
        {
            name: "Dart",
            url: "https://dart.dev",
        },
        {
            name: "Java",
            url: "https://www.oracle.com/in/java/",
        },
        {
            name: "Javascript",
            url: "https://www.javascript.com/",
        },
        {
            name: "Typescript",
            url: "https://www.typescriptlang.org/",
        },
        {
            name: "Microsoft Azure IoTHub",
            url: "https://azure.microsoft.com/en-in/services/iot-hub/",
        },
        {
            name: "Google Firebase",
            url: "https://firebase.google.com/",
        },
        {
            name: "AWS Lambda",
            url: "https://aws.amazon.com/lambda/",
        },
        {
            name: "Espressif ESP32",
            url: "https://www.espressif.com/en/products/socs/esp32",
        },
        {
            name: "Nordic nRF52",
            url: "https://www.nordicsemi.com/Products/Bluetooth-Low-Energy",
        },
        {
            name: "Android",
            url: "https://developer.android.com/",
        },
        {
            name: "Flutter",
            url: "https://flutter.dev/",
        },
    ];
</script>

<section>
    <Heading size="text-2xl">Skills</Heading>
    <div>
        {#each skills as skill}
            <Chip link={skill.url}>{skill.name}</Chip>
        {/each}
    </div>
</section>

<style>
    section {
        padding: 10px 20px;
    }
</style>
