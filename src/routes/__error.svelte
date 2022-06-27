<script context="module" lang="ts">
  /** @type {import('@sveltejs/kit').Load} */
  export function load({ error, status } : {error: {message: string}, status: number}) {
    return {
      props: {
        status: `${status}`,
        message: `${error.message}`
      }
    };
  }
</script>

<script lang="ts">
  export let message: string;
  export let status: number;
</script>

<section class="h-screen flex flex-col justify-center items-center bg-black">
<h1 class="text-9xl font-bold mb-4 text-white">{status}</h1>
<h2 class="text-2xl text-white opacity-50">{message}</h2>
</section>