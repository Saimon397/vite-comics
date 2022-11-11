<template>
    <div class="listMenu">
        <h3>{{ obj.title }}</h3>
        <ul>
            <li v-for="(link, index) in obj.links" :key="index">
                <a :href="link.url">{{ link.text }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ListFooter',
    props: [
        'obj'
    ]
}
</script>

<style lang="scss" scoped>

</style>