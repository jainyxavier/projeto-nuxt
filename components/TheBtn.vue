<template>
    <div>
        <a :href="`${linkBtn}`" :style="{backgroundColor: colorBtn }">{{textBtn}}</a>
    </div>
</template>

<script>
export default {
    name: "TheBtn",
    props: ['textBtn', 'colorBtn', 'linkBtn']
}

</script>

<style lang="scss" scoped>
    div{
        margin-top: 50px;
    }

    a{
        padding: 19px 38px;
        color: #fff;
        text-decoration: none;
        font-size: 1rem;
        font-weight: 500;
        border-radius: 7px;
    }
</style>