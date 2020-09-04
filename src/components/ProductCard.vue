<template>
    <div>
        <vs-row justify="center">
            <vs-col :key="product" v-for="product in products" w="2">
                <vs-card :style="cardStyle">
                    <template #img>
                        <img src="./shared/assets/product2.jpg"></img>
                    </template>
                    <template #text>
                        <h3>{{ product.title }}</h3>
                    </template>
                    <template #interactions>
                        <vs-button danger icon>
                            <i class="bx bx-heart"></i>
                        </vs-button>
                        <vs-button class="btn-chat" shadow>
                            <i class="bx bx-chat"></i>
                            <span class="span">54</span>
                        </vs-button>
                    </template>
                </vs-card>
            </vs-col>
        </vs-row>
    </div>
</template>

<style scoped>
    img {
        height: 200px;
        width: 220px;
    }
</style>

<script>
    export default {
        name: "ProductCard",
        data() {
            return {
                cardStyle: {
                    marginLeft: "20px",
                    flexBasis: "100%"
                },
                products: [
                    {
                        id: 1,
                        title: "iPhone 6 Pro",
                        img: "./shared/assets/product1.jpg"
                    },
                    {
                        id: 2,
                        title: "iPhone 8 Pro",
                    },
                    {
                        id: 3,
                        title: "iPhone 6 Pro",
                    },
                    {
                        id: 3,
                        title: "iPhone 6 Pro",
                    },
                    {
                        id: 3,
                        title: "iPhone 6 Pro",
                    },
                    {
                        id: 3,
                        title: "iPhone 6 Pro",
                    }
                ]
            }
        }
    }
</script>