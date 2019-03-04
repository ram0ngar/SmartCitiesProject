<template>
    <nav class="navbar">
        <button class="navbar__button navbar__button-i">Inicio</button>
        <button class="navbar__button navbar__button-d">Desastres naturales</button>
        <button class="navbar__button navbar__button-a">Emergencia Actual</button>
        <button class="navbar__button navbar__button-b">Blog</button>
    </nav>
</template>

<style lang="scss" scoped>
.navbar {
    background-color: #222831;

    display: flex;
    justify-content: space-evenly;
    align-content: center;
    flex: 0 0 10%;

    &__button {
        border: none;
        background-color: transparent;
        font-size: 1.8rem;
        color: #eeeeee;
        padding: 0.5rem 1rem;
        transition: all 0.2s;
        &-i {
        }
        &-d {
        }
        &-a {
        }
        &-b {
        }
    }

    &__button:hover {
        color: #00adb5;
        transform: translateY(-0.25rem) scale(1.1);
        cursor: pointer;
    }
    &__button:active {
        border: none;
    }
}
</style>

