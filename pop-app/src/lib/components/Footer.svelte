<script lang=ts">
    import { goto } from '$app/navigation';

    import ChatIcon from './chat.svelte';
</script>

<nav>
    <ul>
        <li>
            <button on:click={() => goto('/messaging')}>
                <ChatIcon fill={"purple"}/>
            </button>
        </li>
        <li>
            <button on:click={() => goto('/community')}>
                <img src="/icons/community.svg" alt="Community" class="icon" />
            </button>
        </li>
        <li>
            <button on:click={() => goto('/wallet')}>
                <img src="/icons/wallet.svg" alt="Wallet" class="icon" />
            </button>
        </li>
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
        height: 50px;
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
    .icon {
        width: 2rem;
        height: 2rem;
        margin-bottom: 4px;
    }
</style>