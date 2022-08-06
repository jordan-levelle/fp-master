<template>
    <main class="home-page">
        <div class="tags">
            <h1 class="tag1">hello, i am <br> jordan</h1>
            <p class="tag2"> I am a Creative technologist <br> Welcome to my site</p>
        </div>
            <img class="profileimage" src="../assets/profile.jpg">
    </main>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Fira sans', sans-serif;
    background-color: black;
}

.home-page {
    display: flex;
    align-content: center;
    top: 0;

    animation: fadeInAnimation ease .5s;
            animation-iteration-count: 1;
            animation-fill-mode: forwards;
        }
        @keyframes fadeInAnimation {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
}

.tags{
    display: flex;
    margin-left: 25vw;
    align-items: center;
}

.tag1 {
    color: #fff;
    font-size: 5rem;
    text-transform: uppercase;
}

.tag2 {
    color: #fff;
    font-size: 2rem;
    margin-left: 5rem;

}

.profileimage {
    position: fixed;
    top: 0;
    right: 0;
    height: 100vh;
    width: 55rem;
    object-fit: cover;
    opacity: 0.5;

}
</style>