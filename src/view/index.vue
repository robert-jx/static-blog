<template>
    <div class="home">
        <div class="back-image">
            <section>{{ userinfo.name }}的个人博客</section>
        </div>
        <div class="content">
            <div class="user">
                <div class="head-image">
                    <img src="@/assets/images/user/head.jpg" alt="">
                </div>
                <div class="info">
                    123
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { reactive } from 'vue';
// 配置项内容
export interface userInterface {
    name?: string,
}
let userinfo: userInterface = reactive({
    name: 'robert-jx'
});
</script>

<style lang="scss" scoped>
.home {
    width: 100%;
    height: 100%;

    .back-image {
        width: 100%;
        height: 100%;
        background: url('../assets/images/background/background.jpg') no-repeat;
        background-size: 100% 100%;

        color: #e3e3e3;
        font-size: 48px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-weight: 600;
    }

    .content {
        width: 80%;
        height: 100%;
        margin: 0 auto;
        background-color: #fff;

        .user {
            position: relative;
            width: 100%;
            height: 200px;
            display: flex;
            justify-content: flex-start;
            padding: 0 20px;
            box-sizing: border-box;

            .head-image {
                width: 296px;
                height: 296px;
                transform: translateY(-40%);

                img {

                    width: 296px;
                    height: 296px;
                    border-radius: 50%;
                }
            }

            .info {
                width: calc(100% - 296px);
                height: 100%;
            }
        }
    }
}
</style>