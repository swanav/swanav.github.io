<script>

import Heading from "./components/Heading.svelte";

</script>
<section>
    <Heading size="text-2xl">Education</Heading>

    <ul class="divide-y divide-gray-300">
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="education-row">
                <div>
                    <div class="qualification">Bachelor of Engineering (Electrical Engineering) - AICTE</div>
                    <div class="school">
                        <a href="https://thapar.edu/" target="_blank">Thapar Institute of Engineering and Technology</a>
                    </div>
                    <div class="location">Patiala, Punjab, India</div>
                </div>
                <div>
                    <div class="period">July 2015 - Jun 2019</div>
                    <div class="grade">8.81</div>
                </div>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="education-row">
                <div>
                    <div class="qualification">All India Senior School Certificate Examination (PCM with CS) - CBSE</div>
                    <div class="school">
                        <a href="https://www.asnschool.org/asn-sr.sec/" target="_blank">ASN Sr. Sec. School</a>
                    </div>
                    <div class="location">New Delhi, Delhi, India</div>
                </div>
                <div>
                    <div class="period">Apr 2013 - Mar 2015</div>
                    <div class="grade">92.8%</div>
                </div>
            </div>
        </li>
        <li class="p-4 hover:bg-gray-50 cursor-pointer">
            <div class="education-row">
                <div>
                    <div class="qualification">All India Secondary School Certificate Examination - CBSE</div>
                    <div class="school">
                        <a href="https://www.stcolumbas.edu.in/" target="_blank">St. Columba's School</a>
                    </div>
                    <div class="location">New Delhi, Delhi, India</div>
                </div>
                <div>
                    <div class="period">Apr 2011 - Mar 2013</div>
                    <div class="grade">9.8</div>
                </div>
            </div>
        </li>
      </ul>
</section>

<style>
    section {
        padding: 10px 20px;
    }
    .education-row {
        margin-bottom: 20px;
        display: flex;
    }
    .education-row > div:first-child {
        flex-grow: 3;
    }
    .education-row > div:last-child {
        flex-grow: 1;
        text-align: right;
    }
    .qualification {
        font-weight: bold;
    }
    .period {
        font-weight: bold;
    }
    .grade {
        padding: 4px 0px;
        font-weight: lighter;
        font-size: 1.2em;
    }
</style>


