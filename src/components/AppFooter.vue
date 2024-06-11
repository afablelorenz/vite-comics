<template>
<footer>

    <div class="footer-linksContainer">
        <div class="footerLinksList">
            <div class="footer-links" v-for="(group, index) in footerLinks" :key="index">
                <h4>{{ group.title }}</h4>
                <ul>
                    <li v-for="link in group.links" :key="link.text">
                        <a :href="link.url">{{ link.text }}</a>
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
                <p>facebook</p>
                <p>twitter</p>
                <p>youtube</p>
                <p>pinterest</p>
                <p>maps</p>
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
                    title: 'DC Comics',
                    links: [
                        { text: 'Characters'},
                        { text: 'Comics'},
                        { text: 'Movies'},
                        { text: 'TV'},
                        { text: 'Games'},
                        { text: 'Videos'},
                        { text: 'News'},
                    ]
                },
                {
                    title: 'SHOP',
                    links: [
                        { text: 'Shop DC'},
                        { text: 'Shop DC Collectibles'},
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        { text: 'Terms Of Use'},
                        { text: 'Privacy policy (New)'},
                        { text: 'Ad Choices'},
                        { text: 'Advertising'},
                        { text: 'Jobs'},
                        { text: 'Subscriptions'},
                        { text: 'Talent Workshops'},
                        { text: 'CPSC Certificates'},
                        { text: 'Ratings'},
                        { text: 'Shop Help'},
                        { text: 'Contact Us'},
                    ]
                },
                {
                    title: 'Sites',
                    links: [
                        { text: 'DC'},
                        { text: 'MAD Magazine'},
                        { text: 'DC Kids'},
                        { text: 'DC Universe'},
                        { text: 'DC Power Visa'},
                    ],
                }
            ]
        }
    },
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
