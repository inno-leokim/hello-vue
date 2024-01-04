<template>
    <div>
        <div :class="[color,'box']" :style="{width: width + 'px', height: heigth + 'px'}"></div>        
    </div>
</template>

<script>
    export default {
        props: {
            color: { type: String, default: "" }
        },
        data(){
            return {
                width: 40,
                heigth: 40
            }
        }
    }
</script>

<style scoped>
    .box {
        border: 1px solid #000
    }

    .blue {
        background: #009bff;
    }
    .purple {
        background: #8f46ff;
    }
    .green {
        background: #00bcac;
    }
</style>