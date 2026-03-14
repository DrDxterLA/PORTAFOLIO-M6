<template>

<section class="container">

<h2>Portafolio</h2>

<div class="row">

<div
v-for="project in projects"
:key="project.title"
class="col-lg-4 mb-4"
>

<div class="card">

<img :src="project.image">

<div class="card-body">

<h5>{{project.title}}</h5>

<p>{{project.description}}</p>

</div>

</div>

</div>

</div>

</section>

</template>

<script setup>

import projects from '../data/portfolio'

</script>
