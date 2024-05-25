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

<style>
    nav {
        background-color: #333;
        color: white;
        padding: 1 rem;
        position: fixed;
        bottom: 0;
        width: 100%;
    }
    ul {
        list-style: none;
        display: flex;
        justify-content: space-around;
        padding: 0;
        margin: 0;
    }
    li {
        margin: 0 1rem;
    }
    button {
        background: none;
        border: none;
        color: white;
        font-size: 1rem;
        cursor: pointer;
    }
</style>