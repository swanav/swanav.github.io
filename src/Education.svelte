<script>
    import Heading from "./components/Heading.svelte";
    import LinkText from "./components/LinkText.svelte";

    const qualifications = [
        {
            name: "Master of Science (Computer Engineering)",
            institute: "University of Southern California",
            institute_url: "https://usc.edu",
            location: "Los Angeles, CA, United States",
            period: {
                from: "Aug 2022",
            },
        },{
            name: "Bachelor of Engineering (Electrical Engineering)",
            accredition_organisation: "AICTE",
            institute: "Thapar Institute of Engineering and Technology",
            institute_url: "https://thapar.edu",
            location: "Patiala, Punjab, India",
            period: {
                from: "July 2015",
                to: "Jun 2019",
            },
            grade: "8.81",
        },
        {
            name: "All India Senior School Certificate Examination (PCM with CS)",
            accredition_organisation: "CBSE",
            institute: "ASN Sr. Sec. School",
            institute_url: "https://www.asnschool.org/asn-sr.sec",
            location: "New Delhi, Delhi, India",
            period: {
                from: "Apr 2013",
                to: "Mar 2015",
            },
            grade: "92.8%",
        },
        {
            name: "All India Secondary School Certificate Examination",
            accredition_organisation: "CBSE",
            institute: "St. Columba's School",
            institute_url: "https://www.stcolumbas.edu.in",
            location: "New Delhi, Delhi, India",
            period: {
                from: "Apr 2011",
                to: "Mar 2013",
            },
            grade: "9.80",
        },
    ];
</script>

<section>
    <Heading size="text-2xl">Education</Heading>

    <ul class="divide-y divide-gray-300">
        {#each qualifications as qualification}
            <li class="p-4 hover:bg-gray-50 cursor-pointer">
                <div class="education-row">
                    <div>
                        <div class="qualification">
                            {qualification.name} {#if qualification.accredition_organisation} 
<span> - {qualification.accredition_organisation}</span> {/if}
                        </div>
                        <div class="school">
                            <LinkText url={qualification.institute_url}
                                >{qualification.institute}</LinkText
                            >
                        </div>
                        <div class="location">{qualification.location}</div>
                    </div>
                    <div>
                        <div class="period">
                            {qualification.period.from} - {qualification.period
                                .to ?? "Present"}
                        </div>
                        {#if qualification.grade}<div class="grade">{qualification.grade}</div>{/if}
                    </div>
                </div>
            </li>
        {/each}
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
