<template>
    <div class="project">
        <div class="card">
            <img src="" alt="">
            <div class="links">
                <a href="http://" target="_blank" class="underline">View Live Site</a>
                <a href="http://" target="_blank" class="underline">View Code</a>
            </div>
            <p class="title">project Title</p>
            <div class="skills">
                <p>HTML</p>
                <p>CSS</p>
                <p>JS</p>
            </div>
        </div>
        
        <div class="card">
            <img src="" alt="">
            <div class="links">
                <a href="http://" target="_blank" class="underline">View Live Site</a>
                <a href="http://" target="_blank" class="underline">View Code</a>
            </div>
            <p class="title">project Title</p>
            <div class="skills">
                <p>HTML</p>
                <p>CSS</p>
                <p>JS</p>
            </div>
        </div>

        <div class="card">
            <img src="" alt="">
            <div class="links">
                <a href="http://" target="_blank" class="underline">View Live Site</a>
                <a href="http://" target="_blank" class="underline">View Code</a>
            </div>
            <p class="title">project Title</p>
            <div class="skills">
                <p>HTML</p>
                <p>CSS</p>
                <p>JS</p>
            </div>
        </div>

        <div class="card">
            <img src="" alt="">
            <div class="links">
                <a href="http://" target="_blank" class="underline">View Live Site</a>
                <a href="http://" target="_blank" class="underline">View Code</a>
            </div>
            <p class="title">project Title</p>
            <div class="skills">
                <p>HTML</p>
                <p>CSS</p>
                <p>JS</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .project {
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        gap: 1.4em;
        padding: 4em;

    }

    .card {
        cursor: pointer;
        position: relative;
    }

    img {
        display: block;
        width: 540px;
        height: 400px;
        z-index: 1;
    }

    .card:before {
        content:"";
        position:absolute;
        width:100%;
        height: 400px;
        top:0;left:0;right:0;
        background-color:rgba(0,0,0,0);
        z-index: 2;
    }

    .card:hover::before {
        background-color:rgba(0,0,0,0.1);
    }
   
    .links {
        position: absolute;
        top: 36%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 1.4em;
        padding: 1em;
        opacity: 0;
        z-index: 3;
    }
    .card:hover .links {
        opacity: 1;
    }

    a {
        text-transform: uppercase;
        font-size: 1.125;
    }
   

    .title {
        font-size: 1.5rem;
    }

    .skills {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        gap: 1.2em;
        
    }
</style>