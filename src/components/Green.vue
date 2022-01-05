<template>
    <div>
         <slot name="green">
             <h3>Atlas</h3>
             <p>Lorem ipsum dolor sit amet.</p>
         </slot>
    </div>
</template>

<script>

</script>

<style scoped>
    div {
        border: 1px solid green;
        background-color: lightgreen;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>