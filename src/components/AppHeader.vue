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
    padding:10px 0
}
</style>