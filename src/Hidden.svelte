<script>
    import { createEventDispatcher } from 'svelte';

let shown = false;

    let dispatch = createEventDispatcher();

  export function show() {
    shown = !shown;
            dispatch('show', shown);
    }
</script>