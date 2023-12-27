<template>
    <div class="Person">
        <h2>姓名：{{name}}</h2>
        <h2>年龄：{{ age }}</h2>
        <button @click = showTel>showTel</button>
    </div>
</template>

<script lang="ts">
export default {
    name: 'Person',
    data() {
        return {
            name: 'zhangsan',
            age: 19,
            tel:1111111
        }
    },
    method: {
        showTel() {
            console.log(this.tel)
        }
    }
}

</script>

<style>
.app {
    background-color: #ddd;
    box-shadow: 0 0 10px;
    border-radius: 10px;
    padding: 20px;
}
</style>