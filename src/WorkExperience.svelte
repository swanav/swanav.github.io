<script lang="ts">
    import { fade } from "svelte/transition";
    import Heading from "./components/Heading.svelte";
    import LinkText from "./components/LinkText.svelte";
    let detailView: string | undefined = undefined;
    const clickRow = (role_id: string) => {
        detailView = detailView == role_id ? undefined : role_id;
    };
</script>

<section>
    <Heading size="text-2xl">Work Experience</Heading>
    <ul class="divide-y divide-gray-300">
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div
                class="work-experience-row"
                on:click={() => clickRow("embedded-software-intern-tesla")}
            >
                <div>
                    <div class="qualification">
                        Embedded Software Intern (Gateway)
                    </div>
                    <div class="company">
                        <LinkText url="https://www.tesla.com/"
                            >Tesla, Inc.</LinkText
                        >
                    </div>
                    <div class="location">Palo Alto, California, United States of America</div>
                </div>
                <div>
                    <div class="period">May 2023 - Aug 2023</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    
                </ul>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div
                class="work-experience-row"
                on:click={() => clickRow("senior-firmware-engineer-eran")}
            >
                <div>
                    <div class="qualification">
                        Senior Firmware Engineer (Connected Products)
                    </div>
                    <div class="company">
                        <LinkText url="https://www.eranindustrial.com/"
                            >Eran Innovations LLP</LinkText
                        >
                    </div>
                    <div class="location">Pune, Maharashtra, India</div>
                </div>
                <div>
                    <div class="period">Sep 2020 - Jul 2022</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>
                        Developed and tested ﬁrmware for <LinkText
                            url="https://www.wi-fi.org">Wi-Fi</LinkText
                        > and <LinkText
                            url="https://www.bluetooth.com/blog/introducing-bluetooth-mesh-networking"
                            >BLE Mesh</LinkText
                        > enabled Smart Devices, with a bundled HTTP Server, Websocket
                        Server, <LinkText
                            url="https://azure.microsoft.com/en-in/services/iot-hub"
                            >Azure IoTHub Client</LinkText
                        >, OTA updates and support for <LinkText
                            url="https://www.apple.com/in/ios/home/accessories"
                            >Apple HomeKit</LinkText
                        >, <LinkText
                            url="https://assistant.google.com/smart-home"
                            >Google Home</LinkText
                        > and <LinkText
                            url="https://developer.amazon.com/en-US/alexa/devices/connected-devices"
                            >Amazon Alexa</LinkText
                        > voice assistants.
                    </li>
                    <li>
                        Designed the architecture and Developed Bluetooth Low
                        Energy and Mesh applications for Low Power Devices.
                    </li>
                    <li>
                        Developing a Linux based Connected Camera, with support
                        for Cloud Based Multimedia Stream sharing and sharing of
                        ML telemetry.
                    </li>
                </ul>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div
                class="work-experience-row"
                on:click={() => clickRow("engineer-havells")}
            >
                <div>
                    <div class="qualification">
                        Engineer (Connected Products)
                    </div>
                    <div class="company">
                        <LinkText url="https://havells.com"
                            >Havells India Limited, Centre for Research and
                            Innovation</LinkText
                        >
                    </div>
                    <div class="location">Noida, Uttar Pradesh, India</div>
                </div>
                <div>
                    <div class="period">Jun 2019 - Sep 2020</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>
                        Developed, tested, QA, and assisted in commercialization
                        of ﬁrmware for Connected Smart Fans; Havells <LinkText
                            url="https://www.havells.com/en/consumer/fans/ceiling-fans/smart-fan/carnesia-i-(1).html"
                            >Carnesia-i</LinkText
                        >
                        and <LinkText
                            url="https://www.havells.com/en/consumer/fans/ceiling-fans/smart-fan/stealth-wood-i-walnut-chr.html"
                            >Stealthwood-i</LinkText
                        >. (First such in-house development). These products are
                        now commercially available.
                    </li>
                    <li>
                        Working on designing and implementing a Multi-protocol
                        Smart Hub device with edge intelligence for <LinkText
                            url="https://www.wi-fi.org">Wi-Fi</LinkText
                        >, <LinkText url="https://www.bluetooth.com"
                            >BLE</LinkText
                        >, and <LinkText
                            url="https://zigbeealliance.org/solution/zigbee"
                            >Zigbee</LinkText
                        > devices to enable support for Heterogeneous Mesh networking.
                    </li>
                    <li>
                        Building a customized Embedded Linux solution using the <LinkText
                            url="https://www.yoctoproject.org/"
                            >Yocto build system</LinkText
                        >.
                    </li>
                    <li>
                        Use industry standards-based like <LinkText
                            url="https://openconnectivity.org/">OCF</LinkText
                        >,
                        <LinkText
                            url="https://zigbeealliance.org/solution/dotdot/"
                            >DotDot (ZCL)</LinkText
                        > to maintain interoperability with devices from other manufacturers.
                    </li>
                    <li>
                        Contributed to Architecture design for an IoT Platform
                        based on <LinkText url="https://azure.microsoft.com"
                            >Microsoft Azure Cloud Platform</LinkText
                        >.
                    </li>
                    <li>
                        Developed PoCs for various technologies like <LinkText
                            url="https://developer.amazon.com/en-US/alexa/devices/alexa-built-in"
                            >Alexa Built-in Devices using AVS</LinkText
                        >, <LinkText
                            url="https://developer.amazon.com/en-IN/alexa/alexa-skills-kit"
                            >Alexa Controlled Smart Devices using Alexa Skills
                            Kit</LinkText
                        >, Custom SmartConﬁg implementation, Virtual IoT
                        Devices.
                    </li>
                    <li>
                        Trained all the ﬁrmware developers (10) about the <a
                            href="#hife">ﬁrmware platform</a
                        > and assisted in developing use-cases for various devices.
                        Interviewed (15) candidates for full-time positions in ﬁrmware
                        development.
                    </li>
                </ul>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div
                class="work-experience-row"
                on:click={() => clickRow("intern-havells")}
            >
                <div>
                    <div class="qualification">
                        R&D Intern (Connected Products)
                    </div>
                    <div class="company">
                        <LinkText url="https://havells.com"
                            >Havells India Limited, Centre for Research and
                            Innovation</LinkText
                        >
                    </div>
                    <div class="location">Noida, Uttar Pradesh, India</div>
                </div>
                <div>
                    <div class="period">Jan 2019 - Jun 2019</div>
                </div>
            </div>
            <div class="work-experience-details-row" transition:fade>
                <ul>
                    <li>
                        Developed a <span id="hife">ﬁrmware platform</span> for
                        <LinkText url="https://www.wi-fi.org">Wi-Fi</LinkText
                        >-based IoT devices, incorporating seamless OTA updates, <LinkText
                            url="https://mqtt.org">MQTT</LinkText
                        > for cloud communication, a TCP Server for local cloudless
                        communication,
                        <LinkText
                            url="https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_smartconfig.html"
                            >SmartConﬁg®</LinkText
                        >, and <LinkText
                            url="https://en.wikipedia.org/wiki/Multicast_DNS"
                            >mDNS</LinkText
                        > for seamless device conﬁguration and discovery. This platform
                        will later be used for all the <LinkText
                            url="https://www.wi-fi.org">Wi-Fi</LinkText
                        >-connected devices across the product portfolio with
                        multiple applications in active development.
                    </li>
                    <li>
                        Devised an exhaustive Device Provisioning, Identity
                        Management, and FOTA update policy.
                    </li>
                    <li>
                        Developed, tested, and QA of the <LinkText
                            url="https://www.wi-fi.org">Wi-Fi</LinkText
                        > ﬁrmware along with a user mobile app for a <LinkText
                            url="https://www.wi-fi.org">Wi-Fi</LinkText
                        > Smart AC. (First such in-house development).
                    </li>
                    <li>
                        Developed a cross-platform mobile application (iOS and
                        Android) for the complete IoT device portfolio based on <LinkText
                            url="https://flutter.dev">Flutter</LinkText
                        >.
                    </li>
                    <li>
                        Involved in load-testing of the legacy IoT Cloud
                        Platform using <LinkText url="https://jmeter.apache.org"
                            >Jmeter</LinkText
                        > and customized scripts for simulating virtual devices.
                    </li>
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
