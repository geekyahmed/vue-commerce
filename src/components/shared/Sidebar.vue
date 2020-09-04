<template>
    <div>
        <div class="hidden">
            <vs-sidebar color="#1cc164" absolute hover-expand reduce v-model="active" open>
                <template #logo>
                    <img src="./assets/logo.png" alt="">
                </template>
                <vs-sidebar-item id="home">
                    <template #icon>
                        <i class="bx bx-home"></i>
                    </template>
                    Home
                </vs-sidebar-item>
                <vs-sidebar-item id="home">
                    <template #icon>
                        <i class="bx bx-home"></i>
                    </template>
                    Laptops
                </vs-sidebar-item>
                <vs-sidebar-item id="home">
                    <template #icon>
                        <i class="bx bx-home"></i>
                    </template>
                    TV & Monitors
                </vs-sidebar-item>
                <vs-sidebar-item id="home">
                    <template #icon>
                        <i class="bx bx-home"></i>
                    </template>
                    Computers
                </vs-sidebar-item>
                <vs-sidebar-item id="home">
                    <template #icon>
                        <i class="bx bx-home"></i>
                    </template>
                    Electronics
                </vs-sidebar-item>
            </vs-sidebar>
        </div>
    </div>
</template>

<style scoped>
    div {
        margin-top: 55px;
    }
</style>

<script>
    export default {
        name: "Sidebar",
        data: () => ({
            active: 'home',
        })
    }
</script>