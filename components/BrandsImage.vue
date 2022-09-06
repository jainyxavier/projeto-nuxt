<template>
    <div>
        <div class="box-brand">
            <nuxt-img v-bind:src="`${url}`" />
        </div>
    </div>
</template>

<script>
export default {
    name: 'BrandsImage',
    props: ['url']
}
</script>