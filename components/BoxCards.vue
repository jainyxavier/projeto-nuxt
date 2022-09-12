<template>
    <div class="card">
        <div class="card-info">
            <span>{{title}}</span>
            <h3>{{description}}</h3>
        </div>

        <div class="img-card">
            <nuxt-img :src="`${image}`" />
        </div>
    </div>
</template>

<script>
export default {
    name: "BoxCards",
    props: ['title', 'description', 'image']
}
</script>