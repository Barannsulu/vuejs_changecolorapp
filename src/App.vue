<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button @click="selectedComponent = 'appBlue'" class="btn btn-primary">Mavi Temayı Yükle</button>
                <button @click="selectedComponent = 'appGreen'" class="btn btn-success">Yeşil Temayı Yükle</button>
                <button @click="selectedComponent = 'appRed'" class="btn btn-danger">Kırmızı Temayı Yükle </button>
                <hr>


                <component :is="selectedComponent"></component>

            </div>
        </div>
    </div>
</template>

<script>
    import Blue from './components/Blue.vue';
    import Green from './components/Green.vue';
    import Red from './components/Red.vue';

    export default {
        components: {
            appBlue: Blue,
            appGreen: Green,
            appRed: Red
        },
        
        data : function(){
            return {
                selectedComponent : "appBlue"
            }
        }
    }
</script>

<style>
</style>

