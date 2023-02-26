<script>
  import { Button, Dialog } from "@codepiercer/svelte-tailwind"

  let dialog
</script>

<div class="flex h-screen w-full max-w-none flex-col items-center justify-center gap-2">
  <h1>Welcome to SvelteKit</h1>
  <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
  <Button on:click={dialog.show}>Do not click me!</Button>
</div>

<Dialog bind:dialog closeOnOverlayClick>
  <div slot="content">
    <img
      src="https://media.giphy.com/media/lgcUUCXgC8mEo/giphy.gif"
      alt="rick roll"
      class="mx-auto"
    />
  </div>
</Dialog>
