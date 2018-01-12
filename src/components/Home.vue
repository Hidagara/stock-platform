<template>
    <div>
        <h1>Торгуйте акциями или просмотрите свой портфель</h1>
        <h6>Вы можете сохранить ваши данные</h6>
        <h6>Нажмите "Закончить день" для начала нового дня</h6>
        <hr>
        <p>Ваши средства: {{ funds | currency }}</p>
    </div>
</template>

<script>
    export default {
        computed: {
            funds() {
                return this.$store.getters.funds;
            }
        }
    }
</script>