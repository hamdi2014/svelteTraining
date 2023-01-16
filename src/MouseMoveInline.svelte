<script>
    let m = {x: 0, y: 0};
</script>

<div on:mousemove="{event => m = {x:event.clientX, y:event.clientY}}">
    The mouse position is {m.x} x {m.y}
</div>