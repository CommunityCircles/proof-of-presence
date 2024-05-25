<script lang=ts">
    import { goto } from '$app/navigation';
</script>

<nav>
    <ul>
        <li><button on:click={() => goto('/messaging')}>Chat</button></li>
        <li><button on:click={() => goto('/community')}>Community</button></li>
        <li><button on:click={() => goto('/wallet')}>Wallet</button></li>
    </ul>
</nav>