<script lang="ts">
  export let link: string;
  export let text: string;
</script>

<a
class="unstyled dlp text-white no-underline"
href={link}
rel="noreferrer"
>
{text}
</a>

<style lang="postcss">
  .dlp {
    text-decoration: none;
    font-family: 'Open Sans';
    font-weight: 600;
  }
</style>
