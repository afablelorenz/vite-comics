<script>
export default{
    data(){
        return{
            navLinks:[
                {text: 'Characters'},
                {text: 'Comisc'},
                {text: 'Movies'},
                {text: 'TV'},
                {text: 'Games'},
                {text: 'Collectibles'},
                {text: 'Videos'},
                {text: 'Fans'},
                {text: 'News'},
                {text: 'Shop'},
            ]
        }
    }
}

</script>
<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png">
        </div>
        <nav>
            <ul>
                <li v-for="link in navLinks" :keys="link.text">
                    <a href="">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg">
        </div>
        
    </header>
</template>

<style scoped>

header{
    background-color: white;
    display: flex;
    flex-direction: column;
}

header div.jumbotron{
    width: 100%;
}

div.jumbotron img{
    height: 50vh;
    width: 100%;
}

nav ul{
    height: 10vh;
    display: flex;
    list-style: none;
    align-items: center;
    justify-content: center;
}

nav a{
    color: black;
    text-decoration: none;
    margin: 1rem;
}
</style>