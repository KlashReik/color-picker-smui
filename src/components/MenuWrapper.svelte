<script lang="ts">
  import Menu from "@smui/menu";

  export let wrapper: HTMLElement;
  export let isOpen: boolean = true;
  export let isDialog: boolean = true;
  let menu: Menu;
</script>

<div
  class="mdc-menu mdc-menu-surface smui-menu-surface--static"
  bind:this={wrapper}
  class:isOpen
>
  <slot />
</div>

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
