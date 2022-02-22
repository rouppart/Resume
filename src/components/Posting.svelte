<script lang="ts">
  export let organization: string;
  export let position: string = null;
  export let url: string = null;
  export let location: string = null;
  export let startDate: string;
  export let endDate: string = null;

  let hide = false;

  function switchHide() {
    hide = !hide;
  }
</script>

{#if hide}
<div class="border-2 py-1 text-gray-500 text-center print:hidden" on:click={switchHide}>{organization}</div>
{:else}
<div>
  <div class="flex justify-between space-x-2">
    <div>
      <div class="font-bold cursor-pointer" on:click={switchHide}>{organization}</div>
      {#if position}<div class="font-bold text-gray-500">{position}</div>{/if}
      {#if url}<a href="http://{url}" target="_blank">{url}</a>{/if}
    </div>

    <div class="flex flex-col items-end font-light text-sm tracking-tighter mb-1">
      <div class="w-max">{startDate} {#if endDate} &#8883; {endDate}{/if}</div>
      {#if location}<div class="w-max">{location}</div>{/if}
    </div>
  </div>

  <div class="leading-snug mt-1">
    <slot />
  </div>
</div>
{/if}