
<script>
  import { url, params } from "@roxi/routify";

  const { entity } = $params;

  $: id = $params.edit;
</script>

<div class="page">
  <h2>Entity: {entity}</h2>
  <h3>Edit: {id}</h3>
  <div>    
    <a href={$url('../../')}>Go back</a>
  </div>
</div>

