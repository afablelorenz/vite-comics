<script>

export default{
    data(){
        return{
            blueSectionItems: [
                {name: 'Digital Comics', icon: "../assets/img/buy-comics-digital-comics.png"},
                {name: 'DC Merchandise', icon: '../assets/img/buy-comics-merchandise.png'},
                {name: 'Subscribe', icon: '../assets/img/buy-comics-shop-locator.png'},
                {name: 'Comic Shop Locator', icon: '../assets/img/buy-comics-subscriptions.png'},
                {name: 'DC Power Visa', icon: '../assets/img/buy-comics-buy-dc-power-visa.png'},
            ]
        }
    },
};

</script>
<template>
<main>
    <div class="content-placeholder">
        <p>-->Content goes here <--</p>
    </div>
    <section class="blue-section">
            <!-- <div class="blue-section-item" v-for="item in blueSectionItems" :key="item.name">
            <img :src="item.icon" :alt="item.name">
            <p>{{ item.name }}</p>
            </div>-->
            <ul>
                <li>
                    <img src="../assets/img/buy-comics-digital-comics.png">
                    <p>DIGITAL COMICS</p>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-merchandise.png">
                    <p>DC Merchandise</p>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png">
                    <p>Subscribe</p>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png">
                    <p>Comic Shop Locator</p>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-buy-dc-power-visa.png">
                    <p>DC Power Visa</p>
                </li>
            </ul>
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