<template>
    <div class="service">
        <h4>{{title}}</h4>
        
        <ul>
            <li v-for="item in items">{{item}}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ServicesFooter',
    props: ['title', 'items']
}
</script>