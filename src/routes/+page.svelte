<script lang="ts">
  import MenuWrapper from "../components/MenuWrapper.svelte";
  import Menu from "@smui/menu";
  import ColorPicker from "svelte-awesome-color-picker";
  let open = false;
</script>

<ColorPicker components={{ wrapper: MenuWrapper }} />
<div></div>
<Menu><p>Random paragraph</p></Menu>
