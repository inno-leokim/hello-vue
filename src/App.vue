<template>
    <div>
        <Webtoon :items="webtoons"/>
    </div>
</template>

<script>
import Webtoon from './components/Webtoon.vue';

export default {
    name: 'app',
    components: {
        Webtoon
    },
    data() {
        return {
          webtoons: [
                {
                name: "햄스터와 그녀",
                link: "http://webtoon.daum.net/webtoon/view/hamsterandher",
                img:
                    "http://t1.daumcdn.net/webtoon/op/478cdf37f585607982ffa9e35b432e8503be8a54",
                isUpdate: true
                },
                {
                name: "프롬 스타",
                link: "http://webtoon.daum.net/webtoon/view/fromstar",
                img:
                    "http://t1.daumcdn.net/webtoon/op/a7fb953d722c1130bfc18440f7e3ce448ece57a1",
                isUpdate: true
                },
                {
                name: "위대한 로맨스",
                link: "http://webtoon.daum.net/webtoon/view/greatromance",
                img:
                    "http://t1.daumcdn.net/webtoon/op/a816281cb4df5c50a20ac386fd6e496643d0f085",
                isUpdate: false
                },
                {
                name: "빛나는 손을",
                link: "http://webtoon.daum.net/webtoon/view/Hand",
                img: "http://t1.daumcdn.net/cartoon/5913FCAC0234C50001",
                isUpdate: false
                }
            ] 
        }
    }
}

</script>

<style scoped>
    
</style>