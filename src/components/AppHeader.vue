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
            <img src="../../img/dc-logo.png">
        </div>
        <nav>
            <ul>
                <li v-for="link in navLinks" :keys="link.text">
                    <a href="">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>

header{
    background-color: white;
    padding:10px 0;
    border-bottom: 1px solid #ddd;
    display: flex;
    justify-content: space-around;
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