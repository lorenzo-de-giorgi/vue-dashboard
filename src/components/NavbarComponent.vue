<template>
    <nav>
        <div class="d-flex justify-content-between p-3">
            <div>
                <span><i class="fa-solid fa-bars"></i></span>
            </div>
            <div>
                <span><i class="fa-regular fa-envelope me-3"></i></span>
                <img class="ldg-img" src="../assets/img/user-icon.png">
                <span>Mario Rossi</span>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
nav{
    width: 100%;
}

.ldg-img{
    width: 45px;
    border-radius: 50%;
    border: 1.5px solid white;
}
</style>