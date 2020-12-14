<template>
    <header
        :class="$style.header">
        <div
            :class="[$style['header__container'], 'container']"
        >
            <div
                :class="$style['header__left']">
                <div
                    :class="$style['header__logo']">
                    <img src="~/assets/images/header/logo.svg" alt="Logo">
                </div>
            </div>
            <div
                :class="$style['header__right']">
                <div :class="$style['header__menu']">
                    <div :class="$style['header__item']"></div>
                    <div :class="$style['header__item']"></div>
                    <div :class="$style['header__item']"></div>
                </div>
                <div
                    :class="$style['header__user']"
                >
                    <div
                        :class="$style['header__username']"
                    >Bessie Cooper</div>
                    <img
                        :class="$style['header__avatar']"
                        src="~/assets/images/header/avatar.jpg"
                        alt="Avatar"
                    >
                </div>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        mounted() {
            this.$nextTick(() => {
                console.log(this.$style)
            })
        }
    }
</script>

<style module lang="scss">
    @import "../assets/scss/sections/header";
</style>
