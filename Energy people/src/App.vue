<template>
    <!-- Дана кнопка. Дан массив. Выведите элементы этого массива в виде списка ul. Сделайте так, 
    чтобы по нажатию на кнопку в конец этого списка добавился новый пункт. -->
    <p :class="obj">home</p>
    <button @click="show">show</button>

</template>

<script>
	export default{
        data() {
            return {
                obj: {
                    hidden: true,
                },
            }
        },
        methods: {
            show(){
                this.obj.hidden = !this.obj.hidden;
            }
        }
    }
</script>
<style>

    /* table{
        border-collapse: collapse;
        width: 30%;
        text-align: center;
    }
    td{
        padding: 5px;
        border: 1px solid #000;
    } */
    p.hidden {
	    display: none;
    }

    li{
        color: red;
    }

</style>
