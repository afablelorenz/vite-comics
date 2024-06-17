<template>
<footer>

    <div class="footer-linksContainer">
        <div class="footerLinksList">
            <div class="footer-links" v-for="group in footerLinks" :key="group.title">
                <h4>{{ group.title }}</h4>
                <ul>
                    <li v-for="link in group.links" :key="link">
                        <p>{{ link }}</p>
                    </li>
                </ul> 
        </div>
    </div>
        
        <div>
            <img src="../assets/img/dc-logo-bg.png">
        </div>
    </div>

    <div class="footer2">
        <button>SIGN UP NOW</button>
        <div class="footerSocials">
            <p>FOLLOW US</p>
            <div class="footerSocialsImg">
                <div v-for="social in socialLinks" :key="social.name">
                    <img :src="getImagePath(social.icon)" :alt="social.name">
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default{
    data(){
        return{
            footerLinks: [
                {
                    title: "DC COMICS",
                    links: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
                },
                {
                    title: "SHOP",
                    links: ["Shop DC", "Shop DC Collectibles"],
                },
                {
                    title: "DC",
                    links: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                },
                {
                    title: "SITES",
                    links: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
                }
            ],
            socialLinks: [
                {name: 'Facebook', icon:'../assets/img/footer-facebook.png'},
                {name: 'Facebook', icon:'../assets/img/footer-periscope.png'},
                {name: 'Facebook', icon:'../assets/img/footer-pinterest.png'},
                {name: 'Facebook', icon:'../assets/img/footer-twitter.png'},
                {name: 'Facebook', icon:'../assets/img/footer-youtube.png'},
            ]
        };
    },
    methods:{
        getImagePath: function(imagePath){
            return new URL(imagePath,import.meta.url).href;
        }
    }
};



</script>

<style scoped>

footer{
    width: 100%;
    height: 65.3vh;
    background-image: url('../assets/img/footer-bg.jpg');
    display: flex;
    flex-direction: column;
}

li{
    list-style-type: none;
}
.footer-linksContainer{
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}

.footer-links{
    width: 20vh;
    padding: 1rem;
    display: flex;
    flex-direction: column;
}

.footerLinksList{
    width: 50vw;
    display: flex;
    flex-wrap: wrap;

}

.footer2{
    width: 100%;
    position: absolute;
    bottom: 0;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    background-color: #303030;
}

.footerSocials{
    flex-direction: row;
    display: flex;
    align-items: center;
}
.footerSocials p{
    padding: 0 1rem;
}

.footerSocialsImg{
    display: flex;
    flex-direction: row;
}

.footer2 button{
    margin: 2rem;
    padding: 1rem;
}


</style>
