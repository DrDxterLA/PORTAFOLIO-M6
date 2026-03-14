<template>

<section class="container">

<h2>Habilidades</h2>

<div
v-for="skill in skills"
:key="skill.name"
class="mb-3"
>

<p>{{skill.name}}</p>

<div class="progress">

<div
class="progress-bar"
:style="{width: skill.level + '%'}"
>

{{skill.level}}%

</div>

</div>

</div>

</section>

</template>

<script setup>

import skills from '../data/skills'

</script>