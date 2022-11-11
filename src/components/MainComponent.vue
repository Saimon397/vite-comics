<template>
    <div class="bg-main">
        <div class="container">
            <div class="row">
                <div class="card" v-for="(comic, index) in comics" :key="index">
                    <div class="cardbox">
                        <img :src="comic.thumb" :alt="comic.series">
                    </div>
                    <div>
                        <h4>{{ comic.series }}</h4>
                    </div>
                </div>
            </div>
        </div>
        <div class="btn">
            <button><a href="#nogo">load more</a></button>
        </div>
    </div>
</template>

<script>
import { comics } from '../data/dc-comics';
export default {
    name: 'MainComponent',
    data() {
        return {
            comics: comics
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.bg-main {
    background-color: rgb(28, 28, 28);
}

.container {
    @include dflex
}

.row {
    display: flex;
    flex-flow: row wrap;

    .card {
        margin-top: 50px;
        height: 210px;
        padding: 10px;
        width: calc(100% / 6);

        .cardbox {
            height: 100%;
            overflow-y: hidden;

            img {
                width: 100%;
            }
        }

        div {
            h4 {
                margin-top: 10px;
                text-transform: uppercase;
                color: rgb(254, 252, 241);
                text-align: center;
            }
        }
    }
}

.btn {
    margin-top: 70px;
    text-align: center;

    button {
        background-color: $bluetext;
        height: 40px;
        width: 200px;
        padding: 10px;
        border: none;
        margin-bottom: 10px;
        text-transform: uppercase;
        font-weight: bold;
        font-size: 1em;
        margin-bottom: 30px;

        a {
            color: white;
            text-decoration: none;
        }

        &:hover {
            background-color: rgb(9, 111, 206);
        }
    }
}
</style>