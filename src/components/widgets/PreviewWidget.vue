<template>
    <div class="preview-widget">
        <div class="title">Your Design</div>
        <div class="preview">
            <img class="image-output" src="../../assets/placeholder.png">
        </div>
    </div>
</template>
<script>
export default {
    name: "PreviewWidget",
    props:{}
}
</script>

<style scoped>
    .title{ 
        font-size: 13px;
        font-weight: bold;
        margin-bottom: 10px;
    }
    .preview > .image-output{
        width:100%;
        height: auto;
    }
</style>

