<script lang="ts">
  import { onMount } from 'svelte';
  import { goto } from '$app/navigation';
  import { aStore } from './aStore';

  $: if ($aStore) {
    console.log($aStore);
  }

  onMount(() => goto('/page2'));
</script>
