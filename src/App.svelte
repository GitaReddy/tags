<script>
import Tags from 'svelte-tags-input'
	
// If on:tags is defined
let tag = "";

function handleTags(event) {
    tag = event.detail.tags;
}
</script>

<style>

.my-custom-class {
    width: 500px; /* Adjust the width to your desired size */
  }
  </style>
  
  <div class="my-custom-class">

  <label>Tags</label>
  <br/>

<Tags
    on:tags={handleTags}
   class ="custom-input"
    autoCompleteShowKey={"alpha3Code"}
    autoCompleteKey={"name"}
    maxTags={5}
    placeholder={"Tags Input..."}
    
/>
</div>


