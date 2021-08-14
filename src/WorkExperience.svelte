<section>
    <Heading size="text-2xl">Work Experience</Heading>
    <ul class="divide-y divide-gray-300">
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="work-experience-row" on:click={() => clickRow("senior-firmware-engineer-eran")}>
                <div>
                    <div class="qualification">Senior Firmware Engineer (Connected Products)</div>
                    <div class="company"><a href="https://www.eranindustrial.com/" target="_blank">Eran Innovations LLP</a></div>
                    <div class="location">Pune, Maharashtra, India</div>
                </div>
                <div>
                    <div class="period">Sep 2020 - Present</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>Developed and tested ﬁrmware for WiFi and BLE Mesh enabled Smart Devices, with a bundled HTTP Server, Websocket Server, Azure IoTHub Client, OTA updates and support for Apple Siri, Google Home and Amazon Alexa voice assistant.</li>
                    <li>Designed the architecture and Developed Bluetooth Low Energy and Mesh applications for Low Power Devices.</li>
                    <li>Developing a Linux based Connected Camera, with support for Cloud Based Multimedia Stream sharing and sharing of ML telemetry.</li>
                </ul>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="work-experience-row" on:click={() => clickRow("engineer-havells")}>
                <div>
                    <div class="qualification">Engineer (Connected Products)</div>
                    <div class="company"><a href="https://havells.com" target="_blank">Havells India Limited</a></div>
                    <div class="location">Noida, Uttar Pradesh, India</div>
                </div>
                <div>
                    <div class="period">Jun 2019 - Sep 2020</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>Developed, tested, QA, and assisted in commercialization of ﬁrmware for Wi-Fi Smart Fans; Havells Carnesia-i and Stealthwood-i. (First such in-house development). These products are now commercially available.</li>
                    <li>Working on designing and implementing a Multi-protocol Smart Hub device with edge intelligence for Wi-Fi, BLE, and Zigbee devices with support for Heterogeneous Mesh networking, HSMs.</li>
                    <li>Building a customized Embedded Linux solution using the Yocto build system.</li>
                    <li>Use industry standards-based like <a href="https://openconnectivity.org/" target="_blank">OCF</a>, <a href="https://zigbeealliance.org/solution/dotdot/">DotDot (ZCL)</a> to maintain interoperability with devices from other manufacturers.</li>
                    <li>Contributed to Architecture design for an IoT Platform based on Microsoft’s Azure oﬀerings.</li>
                    <li>Developed PoCs for various technologies like <a href="https://developer.amazon.com/en-US/alexa/devices/alexa-built-in">Alexa Built-in Devices using AVS</a>, <a href="https://developer.amazon.com/en-IN/alexa/alexa-skills-kit">Alexa Controlled Smart Devices using Alexa Skills Kit</a>, Custom SmartConﬁg implementation, Virtual IoT Devices.</li>
                    <li>Trained all the ﬁrmware developers (10) about the ﬁrmware platform and assisted in developing use-cases for various devices. Interviewed (15) candidates for full-time positions in ﬁrmware development.</li>
                </ul>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="work-experience-row" on:click={() => clickRow("intern-havells")}>
                <div>
                    <div class="qualification">R&D Intern (Connected Products)</div>
                    <div class="company"><a href="https://havells.com" target="_blank">Havells India Limited</a></div>
                    <div class="location">Noida, Uttar Pradesh, India</div>
                </div>
                <div>
                    <div class="period">Jan 2019 - Jun 2019</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>Developed a ﬁrmware platform for Wi-Fi-based IoT devices, incorporating seamless OTA updates, MQTT for cloud communication, a TCP Server for local cloudless communication, SmartConﬁg®, and mDNS for seamless device conﬁguration and discovery. This platform will later be used for all the Wi-Fi-connected devices across the product portfolio with multiple applications in active development.</li>
                    <li>Devised an exhaustive Device Provisioning, Identity Management, and FOTA update policy.</li>
                    <li>Developed, tested, and QA of the Wi-Fi ﬁrmware along with a user mobile app for a Wi-Fi Smart AC. (First such in-house development).</li>
                    <li>Developed a cross-platform mobile application (iOS and Android) for the complete IoT device portfolio based on Flutter.</li>
                    <li>Involved in load-testing of the legacy IoT Cloud Platform using Jmeter and customized scripts for simulating virtual devices.</li>
                </ul>
            </div>
        </li>
    </ul>
</section>

<style>

    section {
        padding: 10px 20px;
    }

    .work-experience-row {
        padding: 10px 10px;
        margin-bottom: 20px;
        display: flex;
    }
    .work-experience-details-row {
        /* padding: 10px 20px; */
        margin-bottom: 20px;
        display: flex;
    }

    /* .work-experience-row:hover {
        background-color: #f5f5f5;
    } */
    .work-experience-row > div:first-child {
        flex-grow: 3;
    }
    .work-experience-row > div:last-child {
        flex-grow: 1;
        text-align: right;
    }
    .qualification {
        font-weight: bold;
    }

    .work-experience-details-row > ul {
        list-style-type: disc;
        margin-left: 20px;
    }
</style>

<script lang="ts">
    import { fade } from "svelte/transition"
    import Heading from "./components/Heading.svelte";
    let detailView: string | undefined = undefined;
    const clickRow = (role_id: string) => {
        detailView = detailView == role_id ? undefined : role_id;
    };
</script>
