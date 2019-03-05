<template>
    <main class="landing">
        <div class="bg-video">
            <video class="bg-video__content" autoplay loop muted>
                <source src="./../assets/Dodge-Tornado.mp4" type="video/mp4">
                <source src="./../assets/Dodge-Tornado.webm" type="video/webm">
            </video>
        </div>
         <div class="landing__text-box">
                <h1 class="heading-primary">
                    <span class="heading-primary--main">Natural </span>
                    <span class="heading-primary--sub"
                        >Disasters</span
                    >
                </h1>
            </div>
    </main>
</template>

<style lang="scss" scoped>
.landing {
    display: flex;
    flex: 1;
    position: relative;

    &__text-box {
        position: absolute;
        top: 40%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
    }
}

.bg-video {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: -1;
    opacity: 0.6;
    overflow: hidden;
    &__content {
        height: 100%;
        width: 100%;
        object-fit: cover;
    }
}

@keyframes moveInLeft {
    /*duracion de la animacion*/
    0% {
        opacity: 0;
        transform: translateX(-10rem);
    }

    80% {
        transform: translateX(1rem);
    }

    100% {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes moveInRight {
    0% {
        opacity: 0;
        transform: translateX(10rem);
    }
    80% {
        transform: translateX(-1rem);
    }
    100% {
        opacity: 1;
        transform: translateX(0);
    }
}
.heading-primary {
    color: white;
    text-transform: uppercase;
    /*Evitar el pequeño movimiento del final de la animacion*/
    backface-visibility: hidden;
    margin-bottom: 6rem;

    &--main {
        /*Un bloque ocupa el 100% del ancho */
        display: block;
        font-size: 6rem;
        font-weight: 400;
        letter-spacing: 3.5rem;
        animation-name: moveInLeft;
        animation-duration: 1s;
        /*controlar el tiempo de la animacion, ease-in(rapido al inicio, lento al final)*/
        animation-timing-function: ease-out;
    }

    &--sub {
        display: block;
        font-size: 3rem;
        font-weight: 700;
        letter-spacing: 1.75rem;
        animation: moveInRight 1s ease-out;
    }
}
</style>
