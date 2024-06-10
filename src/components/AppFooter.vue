<template>
<footer>
    <div class="footer-links" v-for="(group, index) in footerLinks" :key="index">
        <h4>{{ group.title }}</h4>
        <ul>
            <li v-for="link in group.links" :key="link.text">
                <a :href="link.url">{{ link.text }}</a>
            </li>
        </ul>
    </div>
    <div>
        <button>SIGN UP NOW</button>
        <div>
            <p>FOLLOW US</p>
            <div>
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
export default {
data() {
    return {
    footerLinks: [
        {
        title: 'DC Comics',
        links: [
            { text: 'Characters', url: '' },
            { text: 'Comics', url: '' },
            { text: 'Movies', url: '' },
            { text: 'TV', url: '' },
            { text: 'Games', url: '' },
            { text: 'Videos', url: '' },
            { text: 'News', url: '' },
        ],
        },
        {
        title: 'DC',
        links: [
            { text: 'Terms Of Use', url: '' },
            { text: 'Privacy policy (New)', url: '' },
            { text: 'Ad Choices', url: '' },
            { text: 'Advertising', url: '' },
            { text: 'Jobs', url: '#' },
            { text: 'Subscriptions', url: '' },
            { text: 'Talent Workshops', url: '' },
            { text: 'CPSC Certificates', url: '' },
            { text: 'Ratings', url: '' },
            { text: 'Shop Help', url: '' },
            { text: 'Contact Us', url: '' },
        ],
        },
        {
        title: 'Sites',
        links: [
            { text: 'DC', url: '' },
            { text: 'MAD Magazine', url: '' },
            { text: 'DC Kids', url: '' },
            { text: 'DC Universe', url: '' },
            { text: 'DC Power Visa', url: '' },
        ],
        },
    ],
    };
},
};
</script>

<style scoped>

footer{
    background-image: url('../assets/img/footer-bg.jpg');
}

</style>
