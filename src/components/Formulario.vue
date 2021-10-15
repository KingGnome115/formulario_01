<template lang="">
    <div class="flex-container">
        <form class="form">
            <div class="form_section">
                <input type="text" class="form_input" placeholder="Nombre Completo">
            </div>
            <div class="form_section">
                <input type="Email" class="form_input" placeholder="Correo Electronico">
            </div>
            <div class="form_section">
                <input type="password" class="form_input" placeholder="Contraseña" title="Una buena contraseña es una frase con espacios, números y simbolos">
            </div>
            <div class="form_section">
                <input type="password" class="form_input" placeholder="Repetir Contraseña" title="Una buena contraseña es una frase con espacios, números y simbolos">
            </div>
            <div class="form_section">
                <input type="tel" class="form_input" placeholder="Número de telefono" title="Una buena contraseña es una frase con espacios, números y simbolos">
            </div>
            <div class="form_section">
                <input type="submit" class="form_input">
            </div>
        </form>
        <div class="form-img">
            <div class="img-container">
                <div>
                    <img src="../assets/imagen.png">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:"Formulario"
    }
</script>

<style scoped>
    .flex-container
    {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        justify-content: center;
        background: #282827;
        margin: 50px 50px;
        padding: 20px;
        border: 14px solid #000;
        outline: 4px solid #D90505;
    }

    .form
    {
        min-width: 400px;
        flex: 1;
        text-align: center;
        padding: 30px;
        order: 5;
    }

    .form_input
    {
        width: 100%;
        padding: 7px;
        margin: 6px 0;
        border: none;
        border-bottom: 3px solid #D90505;
        background: transparent;
        color: #fff;
    }

    .form_input:focus
    {
        background: linear-gradient(to bottom, transparent,#444);
        outline:none;
        border-bottom: 3px solid #720404;
    }

    .form textarea
    {
        min-height: 140px;
        resize: none;
    }

    .form-img
    {
        flex: 1;
        padding: 10px;
        display: flex;
        min-width: 200px;
        order: 2;
    }

    .form-img div
    {
        padding: 20px;
    }

    .img-container
    {
        margin: auto;
    }

    .form-img div
    {
        background: #282827;
        border-radius: 50%;
        text-align: center;
        padding: 30px;
    }

    .form-img img
    {
        width: 80%;
        margin: auto;
    }

    .form input[type="submit"]
    {
        width: 100%;
        background-color: #b10505;
        border-bottom: none;
        padding: 10px;
    }

    .form input[type="submit"]:hover
    {
        background-color: #720404;
        border-bottom: none;
    }

    .form input[type="submit"]:focus
    {
        background-color: #b10505;
        background: linear-gradient(to bottom, #b10505, #720404);
    }

    .form input[type="submit"]:active
    {
        background: linear-gradient(to bottom, #b10505, #720404);
    }

    @media only screen and (max-width: 360px) {
        
        .flex-container
        {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            justify-content: center;
            background: #282827;
            margin: 10px 10px;
            padding: 5px;
            border: 4px solid #D90505;
            outline:  0;
        }

        .form
        {
            min-width: 360px;
            flex: 1;
            text-align: center;
            padding: 30px;
            order: 5;
        }

        .form_input:focus
        {
            background: linear-gradient(to bottom, transparent,#444);
            outline:none;
            border-bottom: 3px solid #720404;
        }

        .form textarea
        {
            min-height: 150px;
        }

        .form-img
        {
            min-width: 300px;
        }

        .img-container
        {
            margin: auto;
        }

        .form-img div
        {
            padding: 10px;
        }

        .form input[type="submit"]
        {
            width: 100.5%;
        }

    }

</style>