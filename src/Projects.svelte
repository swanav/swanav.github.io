<script>

import Heading from "./components/Heading.svelte";

</script>
<section>
    <Heading size="text-2xl">Projects</Heading>
    <div class="project-row">
        <ul class="divide-y divide-gray-300">
            <li class="p-4 hover:bg-gray-50 cursor-pointer">
                <div class="project-title">Overall Student Lead, ThapSat, Student Satellite Program, Thapar Institute of Engineering and Technology, Patiala</div>
                <ul class="project-details">
                    <li>Lead a team of 45 members to develop a student CubeSat.</li>
                    <li>Lead the proposal development of the project for collaboration with the Indian Space Research Organization (ISRO) for technical assistance and payload deployment onto a PSLV.</li>
                    <li>Organized recruitment activities from over 200 applicants for the project from various disciplines of engineering.</li>
                </ul>        
            </li>
            <li class="p-4 hover:bg-gray-50 cursor-pointer">
                <div class="project-title">Remoulding of a Pre-existing Structure into a Smart Building</div>
                <ul class="project-details">
                    <li>Led the proposal development of an INR 3 Crores project submitted to the Department of Science and Technology under the Mission Innovation project in collaboration with Liverpool John Moores University, Liverpool (LJMU) and Indian Institute of Technology, Kanpur (IITK), clearing 2 out of 3 stages of the selection process.</li>
                    <li>The project aims to convert existing oﬀ-grid homes into smart homes using IoT-based retroﬁt modules and optimize energy consumption using machine learning techniques.</li>
                </ul>
            </li>
          </ul>
    </div>
</section>

<style>
    section {
        padding: 10px 20px;
    }
    .project-row {
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