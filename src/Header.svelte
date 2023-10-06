<header>
    <!-- <h1>Swanav Swaroop</h1> -->
    <div>
        <Heading size="text-4xl">Swanav Swaroop</Heading>
    </div>
    <div>
        <div>
            <div class="p-1 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://www.google.com/maps/place/University+of+Southern+California/@34.0192734,-118.2842948,14.96z/data=!4m6!3m5!1s0x80c2c7e49c71a5ed:0xaa905a5bb427a2c4!8m2!3d34.0223519!4d-118.285117!16s%2Fm%2F065y4w7?entry=ttu" target="_blank" rel="noopener">
                    <img id="home-img" src={homeSvg} alt="home"/>
                    <div>
                        Los Angeles, CA
                    </div>
                </a>
            </div>
            <div class="p-1 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="mailto:swanavsw@usc.edu" target="_blank" rel="noopener">
                    <img id="phone-img" src="https://img.shields.io/static/v1?label=&style=for-the-badge&message=swanavsw@usc.edu&color=green&logo=mail" alt="phone"/>
                </a>
            </div>
            <!-- <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="tel:+919821880713">
                    <img id="phone-img" src={phoneSvg} alt="phone"/>
                    <div>
                        <b>+91</b> 9821880713
                    </div>
                </a>
            </div> -->
            <div class="p-1 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="tel:+12139990222" target="_blank" rel="noopener">
                    <img id="phone-img" src="https://img.shields.io/static/v1?label=&style=for-the-badge&message=(213) 999 0222&color=red" alt="phone"/>
                </a>
            </div>
            <!-- <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://linkedin.com/in/swanav" target="_blank" rel="noopener">
                    <img id="linkedin-img" src={linkedSvg} alt="linkedin"/>
                    <div>
                        <span>/in/swanav</span>
                    </div>
                </a>
            </div> -->
            <!-- <div class="badge-base LI-profile-badge" data-locale="en_US" data-size="large" data-theme="dark" data-type="HORIZONTAL" data-vanity="swanav" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://www.linkedin.com/in/swanav?trk=profile-badge"></a></div> -->
            <div class="p-1 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://linkedin.com/in/swanav" target="_blank" rel="noopener">
                    <img id="linkedin-img" src="https://img.shields.io/static/v1?label=&style=for-the-badge&message=swanav&color=blue&logo=linkedin" alt="linkedin"/>
                </a>
            </div>
            <div class="p-1 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://linkedin.com/in/swanav" target="_blank" rel="noopener">
                    <img id="github-img" src="https://img.shields.io/static/v1?label=&style=for-the-badge&message=swanav&color=black&logo=github" alt="github"/>
                </a>
            </div>
            <!-- <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail" >
                <a href="https://github.com/swanav" target="_blank" rel="noopener">
                    <img id="github-img" src={githubSvg} alt="github"/>
                    <div>
                        <span>/swanav</span>
                    </div>
                </a>
            </div> -->
        </div>
    </div>

</header>

<style>


    img {
        max-height: 20px;
        display: inline;
    }
    header {
        display: flex;
    }

    header > div:first-child {
        color: #ff3e00;
        flex-grow: 1;
        vertical-align: middle;
        margin: auto;
        padding-left: 20px;
    }

    header > div:last-child{
        /* flex-grow: 1; */
        align-content: right;
        padding-right: 20px;
    }

    header > div:last-child > div {
        /* display: flex; */

    }

    .icon-detail > a {
        display: flex;
    }

    .icon-detail > a > img {
        /* flex-grow: 1; */
        padding: 0px 10px;
        margin: auto;
    }

    .icon-detail > a > div {
        flex-grow: 1;
    }

</style>

<script lang="ts">
    import Heading from "./components/Heading.svelte";

    import Home from "./icons/home-solid.svg";
    import Phone from "./icons/phone-square-solid.svg";
    import Github from "./icons/github-brands.svg";
    import LinkedIn from "./icons/linkedin-brands.svg";

    const homeSvg = `data:image/svg+xml,${encodeURIComponent(Home)}`; 
    const phoneSvg = `data:image/svg+xml,${encodeURIComponent(Phone)}`; 
    const githubSvg = `data:image/svg+xml,${encodeURIComponent(Github)}`; 
    const linkedSvg = `data:image/svg+xml,${encodeURIComponent(LinkedIn)}`; 
</script>