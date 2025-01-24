<template>
    <div class="CV">
        <div id="title" class="block">
            <div class="face-container">
                <NuxtImg class="face" src="/face.jpg"></NuxtImg>
            </div>
            <div class="text">
                <div class="bold large">Nicholas Bentley</div>
                <div class="quiet">Full-stack Developer<br>& HCI/UX Researcher<br>nic@vaud.uk</div>
            </div>
        </div>
        <div id="intro" class="block">
            <div class="bold">About</div>
            <div>
                Hi, I'm Nic. I enjoy building robust, feature-complete programs and websites to fit user needs. UX oriented with a passion for performant and accessible software. Always tinkering with something.
            </div>
        </div>
        <div id="work-experience" class="block">
            <div class="bold">Work Experience</div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2022 - 2024</div>
                    <NuxtImg class="logo" src="/UoBCrest.png"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">Teaching Assistant<br>University of Birmingham</div>
                    <div>Alongside my PhD, I have been involved in the planning, organisation, teaching, and marking of two final year and masters level university modules - Human-Computer Interaction and Research Topics in HCI.</div>
                    <div class="quiet">Teaching ⬢ Logistics ⬢ Feedback</div>
                </div>
            </div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2018 - 2022</div>
                    <NuxtImg class="logo" src="/mitek.png"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">Software Developer<br>MiTek</div>
                    <div>I worked on multiple projects on worldwide teams and wore many hats at MiTek. Highlights include a full-stack 3D CAD webapp, a legacy CAD desktop app, a web-based logistics/fulfillment platform, and integration between them all. I took lead on a number of features, and also ran workshops to get colleagues up to speed with new technologies.</div>
                    <div class="quiet">C# ⬢ Angular ⬢ HTML5/TS/CSS ⬢ Docker ⬢ Azure ⬢ SQL ⬢ Full-stack</div>
                </div>
            </div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2016</div>
                    <NuxtImg class="logo" src="/xiphos.png"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">Penetration Testing Internship<br>Xiphos Research Ltd.</div>
                    <div>Hands on experience with penetration testing gave me a good understanding of common vulnerabilities, where they come from, and how to prevent them. Getting a look into the guts of a number of systems was invaluable.</div>
                    <div class="quiet">Security ⬢ Performance Profiling ⬢ Network Analysis</div>
                </div>
            </div>
        </div>
        <div id="education" class="block">
            <div class="bold">Education</div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2022 - present</div>
                    <NuxtImg class="logo" src="/UoBCrest.png"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">PhD Study<br>University of Birmingham</div>
                    <div>I am currently pursuing a Human-Computer Interaction PhD. My thesis investigates extending digital fabrication techniques to allow a greater breadth of design space for physical interfaces.</div>
                    
                    <div class="quiet">Papers published:</div>
                    <ul><a class="quiet" href="https://dl.acm.org/doi/10.1145/3654777.3676468">Rhapso: Automatically Embedding Fiber Materials into 3D Prints for Enhanced Interactivity ↗</a></ul>
                    <div class="quiet">HCI ⬢ Interactivity ⬢ Digital Fabrication</div>
                </div>
            </div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2014 - 2018</div>
                    <NuxtImg class="logo" src="/UoBCrest.png"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">MSci Computer Science<br>University of Birmingham</div>
                    <div>Covered a wide variety of topics, specialising in Human-Computer Interaction. My thesis involved the planning, creation, and running of a full-stack testing platform for a study on the interplay between physical and on-screen interfaces.</div>
                    <div class="quiet">Fundamentals ⬢ HCI ⬢ UI/UX ⬢ Interface Research</div>
                </div>
            </div>
        </div>
        <div id="side-projects" class="block">
            <div class="bold">Side Projects</div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">2024 - Ongoing</div>
                    <NuxtImg class="logo" src="/beasties.png"></NuxtImg>
                </div>
                <div class="info">
                    <a class="bold" href="https://belovedbeasties.co.uk">Beloved Beasties ↗</a>
                    <div>A dog walking and pet care company operated by my lovely partner Serin. I manage and host the website on a local server, as well as communications software.</div>
                    <div class="quiet">NuxtJS ⬢ Cloudflare ⬢ Server Hosting ⬢ Docker ⬢ GSuite</div>
                </div>
            </div>
            <div class="entry">
                <div class="date">
                    <div class="text quiet">Ongoing</div>
                    <NuxtImg class="logo face" src="/face.jpg"></NuxtImg>
                </div>
                <div class="info">
                    <div class="bold">This website</div>
                    <div>I've had this site for a while, and enjoy tinkering with it and hosting little projects on subdomains every now and then. Having a local server lets me spin things up and down as much as I feel like it.</div>
                    <div class="quiet">NuxtJS ⬢ Cloudflare ⬢ Server Hosting ⬢ Docker</div>
                </div>
            </div>
        </div>
        <div id="Links" class="block">
            <div class="bold">Links</div>
            <div>
                <ul><NuxtImg class="link-image" src="/github.svg"></NuxtImg> Github - <a href="https://github.com/Vaudrain" target="_blank">@Vaudrain ↗</a></ul>
                <ul><NuxtImg class="link-image" src="/orcid.png"></NuxtImg>ORCID - <a href="https://orcid.org/my-orcid?orcid=0000-0003-0381-4221" target="_blank">0000-0003-0381-4221 ↗</a></ul>
                <ul><NuxtImg class="link-image" src="/linkedin.webp"></NuxtImg><a href="https://www.linkedin.com/in/nic-b-9a03b8157/" target="_blank">LinkedIn ↗</a></ul>
                <ul><NuxtImg class="link-image" src="/CV.png"></NuxtImg><a href="/CV-Nicholas-Bentley.pdf" target="_blank">CV / Resume ↗</a></ul>
                <ul><NuxtImg class="link-image" src="/email.png"></NuxtImg>email - <a href="mailto: nic@vaud.uk" target="_blank">nic@vaud.uk ↗</a></ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;

.CV {
    max-width: 1500px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
}

.block {
    width: 100%;
    max-width: 600px;
    background-color: colours.$transparent-background;
    color: colours.$text;
    margin: 5px;
    padding: 8px;
    border-radius: 5px;
    text-wrap: balance;
}

.face {
    border-radius: 18px;
}

#title {

    display: flex;
    flex-direction: row;

    .face-container {
        background-image: linear-gradient(to bottom right, colours.$accent2 0%, colours.$accent 150%);
        padding: 2px;
        border-radius: 18px;
        

        .face {        
            z-index: 1;
            display: flex;
            justify-content: center;
            height: auto;
            max-height: 120px;
            max-width: 100%;
            border-radius: 18px;
        }
    }

    .text {
        flex-grow: 1;
        align-content: center;
        justify-content: center;
        text-align: center;
    }
}

.entry {
    display: grid;
    grid-template-columns: repeat(4,1fr);

    .date {
        text-align: left;
        display: grid;
        flex-direction: column;

        .text {
            width: 100%;
        }

        .logo {
            width: 50%;
            justify-self: center;
        }
    }

    .info {
        grid-column: span 3/span 3;
    }

}

ul {
    display: flex;
    gap: 10px;
    align-items: center;
    

    .link-image {
        height: 1.5lh;
        width: 1.5lh;
    }
}

</style>