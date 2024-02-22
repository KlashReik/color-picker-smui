<script lang="ts">
  import Menu from "@smui/menu";

  export let wrapper: HTMLElement;
  export let isOpen: boolean = true;
  export let isDialog: boolean = true;
</script>

<Menu open={isOpen}>
  <slot />
</Menu>

<style>
  div {
    display: none;
    width: max-content;
  }
  .isOpen {
    display: block;
  }
  .isDialog {
    position: absolute;
    top: 30px;
    z-index: var(--picker-z-index, 2);
  }
</style>
