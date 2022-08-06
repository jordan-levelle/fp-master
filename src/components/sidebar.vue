<template>
    <aside :class="`${menu_expanded ? 'menu-expanded' : ''}`">
        <div class="logo">
            <img src="../assets/menupic.jpg" alt="">
        </div>

        <div class="menu-toggle-wrap">
            <button class="menu-toggle" @click="ToggleMenu">
                <span class="material-icons">keyboard_double_arrow_right</span>
            </button>
        </div>
           <h3>Menu</h3>
        <div class="menu">
            <router-link class="button" to="/">
                <span class="material-symbols-outlined">home</span>
                <span class="text">Home</span>
            </router-link>
            <router-link class="button" to="/about">
                <span class="material-symbols-outlined">person</span>
                <span class="text">About</span>
            </router-link>
            <router-link class="button" to="/projects">
                <span class="material-symbols-outlined">folder_copy</span>
                <span class="text">Projects</span>
            </router-link>
            <router-link class="button" to="/resume">
                <span class="material-symbols-outlined">Description</span>
                <span class="text">Resume</span>
            </router-link>
            <router-link class="button" to="/contact">
                <span class="material-symbols-outlined">mail</span>
                <span class="text">Contact</span>
            </router-link>
        </div>
    </aside>
</template>

<script setup>
import { ref } from 'vue'

const menu_expanded = ref(localStorage.getItem("menu_expanded") === "true")

const ToggleMenu = () => {
    menu_expanded.value = !menu_expanded.value

    localStorage.setItem("menu_expanded", menu_expanded.value)
}

</script>

<style lang="scss" scoped>
aside {
    display: flex;
    flex-direction: column;
    width: calc(2rem + 32px);
    
    overflow: hidden;
    min-height: 100vh;
    padding: 1rem;

    background-color: var(--dark);
    color: var(--light);

    transition: 0.2s ease-out;

    .logo {
        margin-bottom: 1rem;

        img {
            width: 2rem;
        }
    }

    .menu-toggle-wrap{
        display: flex;
        justify-content: flex-end;
        margin-bottom: 1rem;

        position: relative;
        top: 0;
        transition: 0.2s ease-out;

        .menu-toggle {
            transition: 00.2s ease-out;

            .material-symbols-outlined {
                font-size: 2rem;
                color: var(--light);
                transition: 00.2s ease-out;
            }

            &:hover {
                .material-symbols-outlined{
                    color: var(--primary);
                    transform: translateX(0.5rem);
                }
            }
        }
    }

    h3, .button .text {
        opacity: 0;
        transition: 0.3s ease-out;
    }

    .menu {
        margin: 0 -1rem;

        .button {
            display: flex;
            align-items: center;
            text-decoration: none;

            padding: 0.5rem 1rem;
            transition: 0.2 ease-out;

            .material-symbols-outlined{
                font-size: 2rem;
                color: #fff;
                transition: 0.2s ease-out;
            }

            .text{
                color: #fff;
                transition: 0.2s ease-out;
            }

            &:hover, &.router-link-exact-active {
                background-color: rgb(133, 133, 133);

                .material-symbols-outlined, .text {
                    color: rgb(65, 78, 97);
                }
            }

            &.router-link-exact-active {
                border-right: 5px solid var(--primary);
            }
        }
    }

    &.menu-expanded {
        width: 300px;

        .menu-toggle-wrap{
            top: -3rem;
            .menu-toggle{
                transform: rotate(-180deg);
            }
        }

        h3, .button .text {
            opacity: 1;         
        }

        h3 {
            color: rgb(27, 30, 34);
            font-size: 0.875rem;
            margin-bottom: .5rem;
            text-transform: uppercase;
        }

        .button {
            .material-symbols-outlined{
                margin-right: 1rem;
            }
        }
    }

    @media (max-width: 768px) {
        position: fixed;
        z-index: 99;
    }
}

</style>