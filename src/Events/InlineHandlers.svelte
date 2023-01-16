<script>
    let m = {x: 0, y: 0};
</script>

<div on:mousemove="{event => m = {x:event.clientX, y:event.clientY}}">
    The mouse position is {m.x} x {m.y}
</div>

<style>
    div {width: 100%; height: 25%;}
</style>