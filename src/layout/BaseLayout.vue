<template>
    <div class="wrapper">
        <el-header height="auto"></el-header>
        <el-container class="container">
            <el-aside></el-aside>
            <el-main class="content">
                <keep-alive v-if="$router.meta.keeplive">
                    <router-view></router-view>
                </keep-alive>
                <router-view v-else></router-view>
            </el-main>
        </el-container>
    </div>
</template>

<script>
export default {
  name: 'BaseLayout'
}
</script>

<style lang="scss" scoped>

</style>
