<script lang="ts">
  import ColorPicker from "svelte-awesome-color-picker";
  import MenuTest from "../components/MenuTest.svelte";
  import MenuWrapper from "../components/MenuWrapper.svelte";
</script>

<div style="display: flex; gap: 100px;">
  <ColorPicker components={{ wrapper: MenuTest }} />

  <ColorPicker components={{ wrapper: MenuWrapper }} />
</div>
