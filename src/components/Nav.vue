<template>
    <header>
        <nav class="navbar">
            <a class="navbar-brand" href="/">
                <span class="cnsh">cnsh</span>
                <span class="dev">.dev</span>
            </a>
            <div class="links">
                <a class="nav-link" href="/">Home</a>
                <a class="nav-link" href="/about">About</a>
                <a class="nav-link" href="mailto:cxnshx@gmail.com">Contact</a>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Nav',
    components: {

    }
}
method: {

}
</script>

<style scoped>
:root {
    --header-link-hover: #d7bfdd;
}

header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 5%;
    z-index: 1;
    background-color: rgba(5, 5, 5, 0.5);
}

.navbar-brand {
    float: left;
    font-size: 1.5em;
    color: #000;
    margin-left: 15px;
    will-change: filter;
    margin-top: auto;
}

.navbar-brand .cnsh {
    color: #9ddcec;
}

.navbar-brand .dev {
    color: #d7bfdd;
}

.navbar {
    position: fixed;
    margin-top: 5px;
    margin-left: 0;
    top: 0;
    width: 100%;
}

.navbar .nav-link {
    color: #9ddcec;
    font-size: 1em;
    font-weight: bold;
    text-transform: lowercase;
    text-decoration: none;
    padding: 10px;
    will-change: filter;
}

.navbar .links {
    margin-top: 5px;
    float: right;
    margin-right: 15px;
}

.nav-link:hover {
    transition: color .2s ease-out;
    transition-property: color;
    transition-duration: .2s;
    transition-timing-function: ease-out;
    transition-delay: 0s;
}

@media (prefers-color-scheme: light) {
    header{
        background:  linear-gradient(to bottom, rgba(5, 5, 5, 1.0) -15%, transparent 200%);
    }
}

</style>