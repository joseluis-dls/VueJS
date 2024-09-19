<script setup>

</script>

<template>

    <header class="py-5 header">
        <div class="container-xl">
            <div class="row justify-content-center justify-content-md-between">

                <div class="col-8 col-md-3">
                    <a href="index.html">
                        <img class="img-fluid" src="/public/img/logo.svg" alt="imagen logo">
                    </a>
                </div>

                <nav class="col-md-6 mt-5 d-flex align-items-start justify-content-end">
                    <div class="carrito">
                        <img src="/public/img/carrito.png" alt="imagen carrito" class="img-fluid">
                        <div id="carrito" class="bg-white p-3">
                            <p class="text-center m-3">El carrito está vacío</p>
                            <div>
                                <table class="w-100 table">

                                    <thead>
                                        <tr>
                                            <th>Imagen</th>
                                            <th>Nombre</th>
                                            <th>Precio</th>
                                            <th>Cantidad</th>
                                            <th></th>
                                        </tr>
                                    </thead>

                                    <tbody>
                                        <tr v-for="">
                                            <td>
                                                <img src="" alt="" class="img-fluid">
                                            </td>
                                            <td>Nombre del producto</td>
                                            <td class="fw-bold">$ 0.00</td>
                                            <td class="flex align-items-start gap-4">
                                                <button 
                                                class="btn btn-dark"
                                                type="button"
                                                onclick="decrementar-cantidad"
                                                >-</button>
                                                <span>Cantidad</span>
                                                <button 
                                                class="btn btn-outline-secondary"
                                                type="button"
                                                onclick="incrementar-cantidad"
                                                >+</button>
                                            </td>
                                            <td>
                                                <button 
                                                class="btn btn-danger"
                                                type="button"
                                                onclick="eliminar-producto"
                                                >Eliminar</button>
                                            </td>
                                        </tr>
                                    </tbody>

                                </table>

                                <p class="text-end">Total a pagar: <span class="fw-bold">$ 0.00</span></p>
                                <button 
                                class="btn btn-dark w-100 mt-3 p-2"
                                type="button"
                                onclick="vaciar-carrito"
                                >Vaciar Carrito</button>

                            </div>
                        </div>
                    </div>
                </nav>

            </div>

            <div class="row mt-5">
                <div class="col-md-6 text-center text-md-start pt-5">
                    <h1 class="display-2 fw-bold">Modelo modelo-guitarra</h1>
                    <p class="mt-5 fs-5 text-white">descripcion-guitarra</p>
                    <p class="text-primary fs-1 fw-black">$ precio-guitarra</p>
                    <button 
                    class="btn btn-primary fs-5"
                    type="button"
                    onclick="agregar-al-carrito"
                    >Agregar al carrito</button>
                </div>
            </div>

        </div>
        <img src="/public/img/header_guitarra.png" alt="imagen guitarra" class="header-guitarra">
    </header>

</template>

<style>
    
</style>