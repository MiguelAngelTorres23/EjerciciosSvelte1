<script>
let name = 'inicio'
let edad = 0
let mensaje = 'inicial'
function set_edad(valor) {
edad = valor
}
function comprobarEdad() {

if (edad >= 18){
(
mensaje = "Acceso permitido"
)
 }
 
else{
    (mensaje = "Menor de edad")
    
}

if (edad >=18 && edad <= 32) mensaje = "Edad Adecuada"

}



</script>
<main>
edad: <input type="number" bind:value={edad}>
<button on:click={comprobarEdad}>Comprobar</button>
<label>mensaje: <input type="text" id="txt_mensaje" bind:value={mensaje}> </label>
</main>
<style>
/* shadows: https://css-tricks.com/snippets/css/css-box-shadow/ */
input {
border: none;
box-shadow: 3px 3px 1px 1px #ccc;;
background-color: khaki
}
</style>
