<template>
    <div>
        <AppHeader />
        <slot />
        <AppFooter />
    </div>
</template>

<style lang="scss">
@font-face {
    font-family: 'Sofia Pro Regular';
    src: url('../public/fonts/sofia-pro/Sofia\ Pro\ Regular\ Az.otf');
}
@font-face {
    font-family: 'Sofia Pro Bold';
    src: url('../public/fonts/sofia-pro/Sofia\ Pro\ Bold\ Az.otf');
}

h1, h2, h3, h4, h5, h6{
    font-family: 'Sofia Pro Bold', sans-serif;
}

:root{
    --bkg-color: #333;
}
body{
    font-family: 'Sofia Pro Regular', sans-serif;
}

.main-btn, .alt-btn{
    padding: 0.5em 1.25em;
    border: none;
    border-radius: 2em;
    cursor: pointer;
    text-decoration: none;
    display: flex;
    align-items: center;
}

.main-btn{
  background-color: white;
  color: #333;
}
.alt-btn{
  background-color: transparent;
  color: white;
  border: 2px solid white;
}
</style>