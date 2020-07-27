<script>
 let nombre = 'ana'


function entraNombre(event){
const valorEntrado = event.target.value
 nombre = valorEntrado

if (nombre === 'joan'){
    alert(`buenos dias, ${name}`)
}

}
</script>
<main>
<h3>Hola {nombre}! </h3>
<input type="text" value={nombre} on:input={entraNombre}>
</main>