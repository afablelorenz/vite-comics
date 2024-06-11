<script>

export default{
    data(){
        return{
            blueSectionItems: [
                {id:1,name: 'Digital Comics', img: "../assets/img/buy-comics-digital-comics.png"},
                {id:2,name: 'DC Merchandise', img: '../assets/img/buy-comics-merchandise.png'},
                {id:3,name: 'Subscribe', img: '../assets/img/buy-comics-subscriptions.png'},
                {id:4,name: 'Comic Shop Locator', img: '../assets/img/buy-comics-shop-locator.png'},
                {id:5,name: 'DC Power Visa', img: '../assets/img/buy-dc-power-visa.svg'},
            ]
        }
    },
    methods:{
        getImagePath: function(imagePath){
            return new URL(imagePath,import.meta.url).href;
        }
    }
};

</script>
<template>
<main>
    <div class="content-placeholder">
        <p>-->Content goes here <--</p>
    </div>
    <section class="blue-section">
            <div class="blue-section-item" v-for="(item,i) in blueSectionItems" :key="item.img">
            <img :src="getImagePath(item.img)" :alt="item.name">
            <p>{{ item.name }}</p>
            </div>
    </section>
</main>
</template>

<style scoped>
.content-placeholder {
    width: 100%;
    background-color: #000;
    color: #fff;
    padding: 2rem 0;
    height: 15vh;
}

li{
    list-style-type: none;;
}
.blue-section {
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-content: center;
    flex-direction: row;
    background-color: #00f;
    color: #fff;
    padding: 20px 0;
}

.blue-section ul{
    display: flex;
    justify-content: space-around;
    align-content: center;
}

.blue-section ul li{
    display: flex;
    align-content: center;
    padding: 1rem;
}

.blue-section ul li p{
    display: flex;
    padding: 1rem;
    justify-content: center;
    align-items: center;
}

</style>