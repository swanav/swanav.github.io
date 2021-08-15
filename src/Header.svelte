<header>
    <!-- <h1>Swanav Swaroop</h1> -->
    <div>
        <Heading size="text-4xl">Swanav Swaroop</Heading>
    </div>
    <div>
        <div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://maps.apple.com/place?q=Omaxe%20Palm%20Greens&auid=10591049270420272818&address=MU,%20Greater%20Noida,%20201310,%20Uttar%20Pradesh,%20India&ll=28.477327,77.559706" target="_blank" >
                    <img id="home-img" src={homeSvg} alt="home"/>
                    <div>
                        PPD-1202, Omaxe Palm Greens <br/>
                        Sector Mu, Greater Noida <br/>
                        Uttar Pradesh - 201310 <br/>
                    </div>
                </a>
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="tel:+919821880713">
                    <img id="phone-img" src={phoneSvg} alt="phone"/>
                    <div>
                        <b>+91</b> 9821880713
                    </div>
                </a>
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail">
                <a href="https://linkedin.com/in/swanav" target="_blank">
                    <img id="linkedin-img" src={linkedSvg} alt="linkedin"/>
                    <div>
                        <span>/in/swanav</span>
                    </div>
                </a>
            </div>
            <div class="p-2 hover:bg-gray-50 cursor-pointer icon-detail" >
                <a href="https://github.com/swanav" target="_blank">
                    <img id="github-img" src={githubSvg} alt="github"/>
                    <div>
                        <span>/swanav</span>
                    </div>
                </a>
            </div>
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