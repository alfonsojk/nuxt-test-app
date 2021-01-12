<template>
    <header class="header">
        <h1 class="text-title">Posts App</h1>
        <nav>
            <ul>
                <li>
                    <nuxt-link to="/">Home</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/posts">Posts</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/about">About</nuxt-link>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style>
    .header{
        background:2c3e50;
        color:#ffff;
        display:flex;
        justify-content: space-between;
        align-items:center;
        padding: 1rem 3rem;
        border-bottom: 1px solid #2ecc71;
    }

    header ul{
        display:flex;
        list-style:none;
    }

    header a{
        color:#fff;
        padding:.3rem 1rem;
        margin-right: .5rem;
        text-decoration:none;
        text-transform: uppercase;
    }

    .header a:hover{
        border:1px solid #bdc3c7;
    }
</style>