<script>
let contador = 0;
function sumarUno() {
contador += 1;
}
</script>
<button on:click={sumarUno}>

<!-- si contador es exactamente igual a 1 se pondra la palabra vez si no es asi la palabra veces -->

Clicked {contador} {contador === 1 ? 'vez' : 'veces'}
</button>

