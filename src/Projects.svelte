<script>
    import Heading from "./components/Heading.svelte";

    const projects = [{
        title: "Overall Student Lead, ThapSat, Student Satellite Program, Thapar Institute of Engineering and Technology, Patiala",
        url: "http://thapsat.thapar.edu",
        features: [
            "Lead a team of 45 members to develop a student CubeSat.",
            "Lead the proposal development of the project for collaboration with the Indian Space Research Organization (ISRO) for technical assistance and payload deployment onto a PSLV.",
            "Organized recruitment activities from over 200 applicants for the project from various disciplines of engineering."
        ]
    }, {
        title: "Remoulding of a Pre-existing Structure into a Smart Building",
        features: [
            "Led the proposal development of an INR 3 Crores project submitted to the Department of Science and Technology under the Mission Innovation project in collaboration with Liverpool John Moores University, Liverpool (LJMU) and Indian Institute of Technology, Kanpur (IITK), clearing 2 out of 3 stages of the selection process.",
            "The project aims to convert existing oﬀ-grid homes into smart homes using IoT-based retroﬁt modules and optimize energy consumption using machine learning techniques."
        ]
    }]

</script>

<section>
    <Heading size="text-2xl">Projects</Heading>
    <div class="projects-row">
        <ul class="divide-y divide-gray-300">
            {#each projects as project}
                <li class="p-4 hover:bg-gray-50 cursor-pointer">
                    <div class="project-title">
                        {#if project.url}
                            <a href={project.url} target="_blank" >{project.title}</a>
                        {:else}
                            {project.title}
                        {/if}
                    </div>
                    <ul class="project-details">
                        {#each project.features as feature}
                        <li>{feature}</li>
                        {/each}
                    </ul>
                </li>
            {/each}
        </ul>
    </div>
</section>

<style>
    section {
        padding: 10px 20px;
    }
    .projects-row {
        margin-bottom: 20px;
    }
    .project-title {
        font-weight: bold;
    }
    .project-details {
        list-style-type: disc;
        margin-left: 20px;
    }
</style>
