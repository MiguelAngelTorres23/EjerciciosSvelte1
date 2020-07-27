<script>
let nombre = 'ana'
let apellido = 'fernandez'
</script>
<main>
<h3>Hola {nombre} {apellido}! </h3>
<p>Pon tu nombre:</p>
<input type="text" bind:value={nombre}>
<p>Pon tu apellido:</p>
<input type="text" bind:value={apellido}>
</main>
