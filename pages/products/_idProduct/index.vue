<template>
    <div>
        <h1>
            El id del producto es {{$route.params.idProduct}}
        </h1>
        <button @click="$router.push('/')"></button>
    </div>
</template>