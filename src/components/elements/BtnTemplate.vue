<template>
    <div class="container-fluid">
        <!-- center -->
        <div class="row ">
            <div class="col-12">
                <button id="btn-template">{{ text }}</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        text: {}
    }

}
</script>

<style>
#btn-template {
    height: 50px;
    width: 45%;
    border-radius: 25px;
    background-image: radial-gradient(circle at 91.6% 38.85%, #fe9362 0, #ff8864 8.33%, #ff7c66 16.67%, #ff6e6a 25%, #fd5f6e 33.33%, #f94f73 41.67%, #f23c78 50%, #ea267f 58.33%, #e00a87 66.67%, #d40090 75%, #c6009b 83.33%, #b600a6 91.67%, #a307b2 100%);
    font-weight: bold;
}
#btn-template:hover{
    background-color: #4746461f;
    background-blend-mode: overlay;
}
</style>