<script lang="ts">
  import Menu from "@smui/menu";
  import List from "@smui/list";

  export let wrapper: HTMLElement;
  export let isOpen: boolean = true;
  export let isDialog: boolean = true;
  let menu: Menu;

  $: console.log(menu);

  $: if (menu) {
    menu.setOpen(isOpen);
  }
</script>

<div bind:this={wrapper}>
  <Menu bind:this={menu} open={false}>
    <List>
      <slot />
    </List>
  </Menu>
</div>

<style>
  /* div {
    display: none;
    width: max-content;
  }
  .isOpen {
    display: block;
  } */
</style>
