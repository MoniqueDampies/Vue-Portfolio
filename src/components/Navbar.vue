<template>
    <header>
        <div id="home"></div>
        <nav class="navbar navbar-expand-sm navbar bg-transparent fixed-top">
            <div class="container">
                <!-- <a class="navbar-brand mb-0 h1" href="#">Monique.</a> -->
                <!-- button -->
                <div class="row">
                    <button class="navbar-toggler text-end justify-content-end" type="button" data-bs-toggle="collapse"
                        data-bs-target="#navbarNav">
                        <span class="navbar-toggler-icon bg-light"></span>
                    </button>
                </div>

                <!-- data -->
                <div class="collapse navbar-collapse justify-content-end" id="navbarNav"
                    style="text-shadow: 5px 3px 4px rgba(193, 185, 193, 0.8);">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link mb-0 h5 " href="#master">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link mb-0 h5 " href="#About">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link mb-0 h5 " href="#resume">Resume</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link mb-0 h5" href="#projects">Projects</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link mb-0 h5" href="#contact">Contact</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Navbar'

}
</script>

<style scoped>
header {
    overflow-x: hidden;
    padding: 0;
    margin: 0;
}

nav {
    overflow-x: hidden;
    width: 100%;
}

.container {
    /* width: 90%; */
}

.nav-item a {
    position: relative;
    text-decoration: none;
}

.nav-item a::before {
    content: '';
    position: absolute;
    /* width: 100%; */
    height: 3px;
    border-radius: 3px;
    background-color: #fbfeff;
    bottom: 0;
    left: 0;
    transform-origin: middle;
    transform: scaleX(0);
    transition: transform .3s ease-in-out;
}

.nav-item a:visited {
    color: white;
    text-shadow: 5px 3px 10px rgba(0, 0, 0, 0.7);
}

.nav-item a:link {
    color: white;
    text-shadow: 5px 3px 10px rgba(0, 0, 0, 0.7);
}

.nav-link a:hover {
    color: #000000;
}

.nav-item a:hover {
    transform-origin: middle;
    transform: scaleX(1.05);
    text-decoration: none;
    color: rgba(16, 14, 14, 0.633) !important;
}

.navbar:hover {
    /* color: #000000; */
    width: 100%;
    background: rgba(255, 255, 255, 0.23);
    border-radius: 16px;
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(16.3px);
    -webkit-backdrop-filter: blur(16.3px);
}

button {
    justify-content: end;
}

@media only screen and (max-width: 790px) {
    .navbar-toggler-icon{
        border-radius: 10rem;
    }
}
</style>