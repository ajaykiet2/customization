<template>
    <div class="text-element">
        <label>{{label}}</label>
        <input type="text" class="textbox">
    </div>
</template>
<script>
export default {
    name: "TextElement",
    props:{
        label:{type: String, default: "Text Component"},
    }
}
</script>
<style scoped>
    .text-element{
        padding:5px;
        margin-bottom:10px;
    }
    .text-element > label{
        font-size: 13px;
    }
    .textbox{
        box-sizing : border-box;
        border:1px solid #ccc;
        padding:5px 10px;
        border-radius: 2px;
        width:100%;
        margin-top:3px;
    }
    .textbox:focus{
        outline:none;
        border:1px solid #AAA;
    }
</style>


