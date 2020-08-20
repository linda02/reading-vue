<template>
    <div class="col-sm-3 col-md-2 sidebar">
        <ul class="nav nav-sidebar">
            <router-link tag="li" to="/applist">
                <a>英雄列表</a>
            </router-link>
            <router-link tag="li" to="/about">
                <a>武器列表</a>
            </router-link>
            <router-link tag="li" to="/foo">
                <a>装备列表</a>
            </router-link>
        </ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {

            }
        },
    }
</script>

<style scoped>

</style>