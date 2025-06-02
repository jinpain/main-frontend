<script>
  import NotifyList from "./NotifyList.svelte";
  import Sidebar from "./Sidebar.svelte";

</script>

<div class="h-100 d-flex justify-content-between">
    <div>
        <Sidebar />
    </div>
    <div>
        <NotifyList></NotifyList>
    </div>
    <div>
        <NotifyList />
    </div>
</div>