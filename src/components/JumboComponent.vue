<template>
    <div>
        <div class="jumbo">
            <button><a href="#nogo">current series</a></button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'JumboComponent',
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.jumbo {
    background-image: url(../../img/jumbotron.jpg);
    background-size: cover;
    height: 45vh;
    background-repeat: no-repeat;
    position: relative;

    button {
        position: absolute;
        left: 200px;
        bottom: -30px;
        border: none;
        background-color: $bluetext;
        height: 55px;
        padding: 10px;

        &:hover {
            background-color: rgb(9, 111, 206);
        }

        a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 1.8em;
        }
    }
}
</style>