<script lang="ts">
  export let name: string;
  import { Accordion, AccordionItem } from "carbon-components-svelte";
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
  <Accordion>
    <AccordionItem title="Section 1" open>Content 1</AccordionItem>
    <AccordionItem title="Section 2">Content 2</AccordionItem>
    <AccordionItem title="Section 3">Content 3</AccordionItem>
  </Accordion>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
