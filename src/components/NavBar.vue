<template>
    <main>
        <header>
            <div class="container">
                <router-link to="/">
                    <img class="logo" src="../assets/logo.png" alt="logo">
                </router-link>

                <nav>
                    <ul>
                        <li><router-link to="/">Home</router-link></li>
                        <li><a href="">One</a></li>
                        <li><a href="">Two</a></li>
                        <li><a href="">Three</a></li>
                        <li><a href="">Four</a></li>
                    </ul> 
                </nav>
            </div>
        </header>
    </main>
</template>

<script>
export default {

}
</script>

<style scoped>
header {
    background: rgb(51, 51, 51);
    font-family: Arial, Helvetica, sans-serif;
}

header::after {
    content: '';
    display: table;
    clear: both;
}

.container {
    width: 80%;
    margin: 0 auto;
}

.logo {
    height: 40px;
    width: 40px;
    float: left;
    padding: 10px 0;
    transition: all ease-in-out 800ms;
    cursor: pointer;
}

.logo:hover {
    transform: rotate(360deg);
}

nav {
    float: right;
}

nav ul {
    margin: 0;
    padding: 0;
    list-style: none;
}

nav li {
    display: inline-block;
    margin-left: 40px;
    padding-top: 20px;
    position: relative;
}

nav a {
    color: rgb(224, 224, 224);
    text-decoration: none;
    text-transform: uppercase;
    transition: all ease-in-out 400ms;
}

nav a:hover {
    color: rgb(0, 225, 255);
}

nav a::before {
    content: '';
    display: block;
    height: 5px;
    background: linear-gradient(to left, rgb(0, 255, 64), rgb(51, 51, 51));
    position: absolute;
    top: 0;
    width: 0%;
    border-radius: 0px 5px 5px 0px;
    transition: all ease-in-out 250ms;
}

nav a:hover::before {
    width: 100%;
}
</style>