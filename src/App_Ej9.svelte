<script>
let name = 'ana'
function saludar() {
cadena = `Buenos dias ${name}`
alert (cadena)
}
$: saludar(name)
</script>
<main>
<h3>Hello {name}! </h3>
<input type="text" bind:value={name}>
</main>

<!-- Cualquier declaración de nivel superior 
(es decir, no dentro de un bloque o una función) se puede hacer reactiva prefijándola con la $:  
.Las declaraciones reactivas se ejecutan inmediatamente antes de que el componente se actualice, 
siempre que los valores de los que dependen hayan cambiado. -->