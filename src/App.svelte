<script lang="ts">
import Header from "./Header.svelte"
import Education from "./Education.svelte";
import WorkExperience from "./WorkExperience.svelte";
import Projects from "./Projects.svelte";
import Skills from "./Skills.svelte";
</script>



<style>
main {
	padding: 1em;
	padding-bottom: 2em;
	margin: 0 auto;
}

@media (min-width: 960px) {
	main {
		width: 960px;
	}
}
</style>

<main>
	<Header/>
	<hr/>
	<Education/>
	<hr/>
	<WorkExperience/>
	<hr/>
	<Projects/>
	<hr/>
	<Skills/>
</main>
