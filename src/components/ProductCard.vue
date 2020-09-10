<template>
    <div>
        <vs-row :style="styles" justify="center" w="12">
            <vs-col sm="8" xs="7">
                <h2 align="center" justify="center"> VueCommere -<span>The Ecommerce UI Built With Vue</span> </h2>
            </vs-col>
            <vs-col :key="product" v-for="product in products" w="3" flex-start lg="3" sm="8" xs="7">
                <vs-card :style="cardStyle">
                    <template #img>
                        <img src="./shared/assets/product2.jpg"></img>
                    </template>
                    <template #text>
                        <h3>{{ product.title }}</h3>
                        <div style="display: flex;">
                            <vs-button flat border secondary>Buy</vs-button>
                            <vs-button flat border>Add To Wishlist</vs-button>
                        </div>
                    </template>
                    <template #interactions>
                        <vs-button danger icon>
                            <i class="bx bx-heart"></i>
                        </vs-button>
                        <vs-button class="btn-chat" shadow>
                            <i class="fa fa-comments"></i>
                            <span class="span">54</span>
                        </vs-button>
                    </template>
                </vs-card>
            </vs-col>
        </vs-row>
    </div>
</template>

<style scoped>
    h2 {
        margin-top: 80px;
        font-size: 30px;
    }

    span {
        color: "#1cc21c";
        font-weight: semi-bold;
    }

    img {
        height: 200px;
        width: 350px;
    }
</style>

<script>
    export default {
        name: "ProductCard",
        data() {
            return {
                cardStyle: {
                    width: "250px",
                    margin: "10px"
                },
                products: [
                    {
                        id: 1,
                        title: "iPhone 6 Pro",
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
                        id: 1,
                        title: "iPhone 6 Pro",
                    },
                    {
                        id: 2,
                        title: "iPhone 8 Pro",
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