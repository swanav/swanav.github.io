<header>
    <!-- <h1>Swanav Swaroop</h1> -->
    <div>
        <Heading size="text-4xl">Swanav Swaroop</Heading>
    </div>
    <div>
        <div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer">
                PPD-1202, Omaxe Palm Greens <br/>
                Sector Mu, Greater Noida <br/>
                Uttar Pradesh - 201310 <br/>
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer">
                +91 9821880713
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer">
                <a href="https://linkedin.com/in/swanav" target="_blank">
                    <img id="linkedin-img" src={linkedInSvg} alt="linkedin"/>
                    <!-- {@html LinkedIn} -->
                    <span>/in/swanav</span>
                </a>
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer">
                <a href="https://github.com/swanav" target="_blank">
                    <img id="github-img" src={githubSvg} alt="github"/>
                    <span>/swanav</span>
                </a>
            </div>
        </div>
    </div>

</header>

<style>

    #linkedin-img {
        color: blue;
    }

    img {
        max-height: 20px;
        display: inline;
    }
    header {
        display: flex;
    }

    header > div:first-child {
        color: #ff3e00;
        font-weight: bold;
        flex-grow: 2;
        vertical-align: middle;
        margin: auto;
    }

    header > div:last-child{
        /* flex-grow: 1; */
        align-content: right;
    }

    header > div:last-child > div {
        /* display: flex; */
    }

    /* h3 {
		color: #ff3e00;
        font-weight: bold;
	} */
</style>

<script lang="ts">
    import Heading from "./components/Heading.svelte";
    import Github from "./icons/github-brands.svg";
    import LinkedIn from "./icons/linkedin-in-brands.svg";
    const githubSvg = `data:image/svg+xml,${encodeURIComponent(Github)}`; 
    const linkedInSvg = `data:image/svg+xml,${encodeURIComponent(LinkedIn)}`; 
</script>