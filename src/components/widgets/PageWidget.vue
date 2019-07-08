<template>
    <div class="pages">
        <div class="title">Pages</div>
        <div class="thumbnails">
            <div class="thumb">
                <img src="../../assets/placeholder.png">
                <p class="name">Frontside</p>
            </div>
            <div class="thumb">
                <img src="../../assets/placeholder.png">
                <p class="name">Backside</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "PageWidget",
    props:{}
}
</script>
<style scoped>
    .pages{
        padding: 0 25px;
    }
    .title { 
        font-size: 13px;
        font-weight: bold;
        margin-bottom: 10px;
    }
    .thumb .name {
        text-align: center;
        color:#999;
        font-size: 10px;
        line-height: 0px;
        padding-bottom:15px;
    }
    .thumbnails img {
        width: 100%;
        height:auto;
    }
</style>


