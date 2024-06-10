<script>
export default{
    data(){
        return{
            blueSectionItems: [
                {name: 'Digital Comics', icon: '../assets/img/buy-comics-digital-comics.png'}
                
            ]
        }
    }
}

</script>
<template>
<main>
    <div class="content-placeholder">
        <!-- Content goes here -->
    </div>
    <section class="blue-section">
        <div class="blue-section-item" v-for="item in blueSectionItems" :key="item.name">
            <img :src="item.icon" :alt="item.name">
            <p>{{ item.name }}</p>
        </div>
    </section>
</main>
</template>
<style>

</style>