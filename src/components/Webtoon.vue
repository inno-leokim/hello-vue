<template>
    <head>
        <!-- <META HTTP-EQUIV="Pragma" CONTENT="no-cache">
        <META HTTP-EQUIV="Expires" CONTENT="-1"> -->
        <meta http-equiv="pragma" content="no-cache">
        <meta http-equiv="Expires" content="-1">
    </head>
    <div>
        <h2>Webtoon</h2>
        <ul class="wrap">
            <li class="item" v-for="(item, idx) in items" :key="{idx}">
                <a :href="item.link" target="_blank">
                    <img :src="item.img" alt="">
                    <span class="tit">제목 {{ item.name }}</span>
                </a>
                <span class="tag" v-if="item.isUpdate">N</span>
            </li>    
        </ul>
    </div>
</template>

<script>
    export default {
        props: {
            items: {type: Array, default: () => []}
        }
    }
</script>

<style scoped>
    h2 {
        text-align: center;
    }

    a {
        list-style: none;
        text-decoration: none;
    }

    li {
        list-style: none;
    }

    .wrap {
        max-width: 450px;
        width: 100%;
        margin: 0 auto;
    }

    .item {
        position: relative;
        border-bottom: 1px solid #ebebeb;
        margin-bottom: 25px;
    }
    .tit {
        display: inline-block;
        font-size: 18px;
        font-weight: bold;
        color: #000;
        padding: 20px 15px;
    }
    .tag {
        position: absolute;
        left: 10px;
        top: 10px;
        padding: 5px 30px;
        color: #fff;
        border-radius: 4px;
        background: #fc2332;
        font-weight: bold;
    }

    img {
        width: 100%;
        background: #ebebeb;
        border-radius: 4px;
    }
</style>