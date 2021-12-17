<template>
    <div id="app" class="main-content" style="height: 100vh">
        <div class="container">
            <div class="row">
                <div class="d-flex justify-content-center align-items-center my-5">
                    <!-- card -->
                    <div
                        @click="selectToken()"
                        class="card align-items-center shadow-lg super-rounded px-4"
                        style="width: 25rem"
                    >
                        <img
                            src="./assets/image-equilibrium.jpg"
                            alt=""
                            class="card-img-top mt-4"
                        />

                        <div class="card-body">
                            <!-- title -->
                            <h2 class="card-title mt-3 text-white change-on-select">
                                Equilibrium #3429
                            </h2>

                            <!-- text -->
                            <p class="card-text text-muted text-light-blue my-4">
                                Our Equilibrium collection promotes balance and coin.
                            </p>

                            <!-- nft content -->

                            <div class="d-flex align-items-center justify-content-between">
                                <!-- ETH  -->
                                <div class="d-flex gap-2 align-items-center">
                                    <img
                                        src="./assets/icon-ethereum.svg"
                                        class="mr-auto"
                                        height="18px"
                                        width="auto"
                                    />

                                    <p class="text-cyan fw-bold mb-0">0.041 ETH</p>
                                </div>

                                <!-- Time Left  -->
                                <div class="d-flex gap-2 align-items-center">
                                    <img
                                        src="./assets/icon-clock.svg"
                                        class="mr-auto"
                                        height="18px"
                                        width="auto"
                                    />

                                    <p class="text-light-blue mb-0">3 days left</p>
                                </div>
                            </div>

                            <!-- linebreak  -->
                            <hr size="3" />

                            <!-- footer; creator info -->

                            <div class="d-flex align-items-center gap-3 my-3">
                                <img
                                    src="./assets/image-avatar.png"
                                    height="30px"
                                    width="30px"
                                    class="avatar-border"
                                />

                                <p class="text-light-blue mb-0">
                                    Creation of
                                    <span class="text-white change-on-select">Jules Wyvern</span>
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "App",
    methods: {
        selectToken() {
            console.log("token selected!");
        },
    },
};
</script>

<style>
#app {
    background-color: #0d192b;
}

.super-rounded {
    border-radius: 10px;
}

.card {
    background-color: #14253d;
}

.text-light-blue {
    color: #8bacda !important;
}

.card-img-top {
    border-radius: 10px;
}

.avatar-border {
    border: 1px solid white;
    border-radius: 15px;
}

.text-cyan {
    color: hsl(178, 100%, 50%);
}

.card:hover {
    transform: scale(1.05);
    cursor: pointer;
}

.card:hover .change-on-select {
    color: aqua !important;
}

.card:hover .card-img-top {
    border: 1px solid aqua;
}

hr {
    color: grey;
}
</style>
