<script setup>
import { RouterLink } from 'vue-router'



</script>
<template>
    <div>
        <div class="container">

            <div class="nav-scroller py-1 mb-3 border-bottom">
                <nav class="nav nav-underline justify-content-between">
                <RouterLink class="nav-item nav-link link-body-emphasis active" to="/">Home</RouterLink>

                <RouterLink class="nav-item nav-link link-body-emphasis" to="/Review">Review</RouterLink>

                <RouterLink class="nav-item nav-link link-body-emphasis" to="/about">About</RouterLink>

                </nav>
            </div>
        </div>
    </div>



</template>
