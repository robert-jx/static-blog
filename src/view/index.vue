<template>
    <div class="home">
        <section class="back-image"></section>
        <section class="content">
            <section class="user">
                <section class="head-image">
                    <img src="@/assets/images/user/head.jpg" alt="">
                </section>
                <section class="info">
                    123
                </section>
            </section>
        </section>
    </div>
</template>

<script setup lang="ts">

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