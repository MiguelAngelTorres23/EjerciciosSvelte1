<script>
let edad = 0, mensaje1 = '-', mensaje2 = '-'
function comprobarEdad() {
if(edad >= 18) mensaje2 = "Mayor de edad"
else
{
mensaje2 = "Menor de edad"
}

if (edad >=119) mensaje2 = "Edad inadecuada"

}
$: if (edad!=0 && edad>9) comprobarEdad()
$: if (edad>0 && edad<9) mensaje2 = "Debe ser mayor que 9"
</script>
<main>
<h3>Máquina de votar</h3>
Edad: <input type="number" bind:value={edad}>
<br>
mensajes:
<input type="text" id="txt_mensaje2" bind:value={mensaje2}>
</main>