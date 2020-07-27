<script>
let ciudad = '-'
let edad = 0
let mensaje1 = '-'
let mensaje2 = '-'
function comprobarEdad() {
edad >= 18 ?
(
mensaje2 = "Mayor de edad"
)
:
(
mensaje2 = "Menor de edad"
)
}
function comprobarCiudad() {
const ciudad_Switch = (valor) => ({
"palma": true,
"calvia":true,
"inca":true,
"manacor":true,
})[valor] || false;
return (ciudad_Switch(ciudad));
}
$: if (edad!=0) comprobarEdad()
$: if (ciudad != '') {
let admitida = comprobarCiudad()
admitida ? mensaje1 = "Ciudad admitida" : mensaje1 = "Ciudad NO correcta"
console.log (mensaje1)
}
</script>
<main>
<h3>Máquina de votar</h3>
Ciudad: <input type="text" bind:value={ciudad}>
Edad: <input type="number" bind:value={edad}>
<br>
mensajes: <input type="text" id="txt_mensaje1" bind:value={mensaje1}>
<input type="text" id="txt_mensaje2" bind:value={mensaje2}>
</main>