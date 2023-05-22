<script>
import Tags from 'svelte-tags-input'
	
// If on:tags is defined
let tag = "";

function handleTags(event) {
    tag = event.detail.tags;
}







</script>

<Tags
    on:tags={handleTags}
   
    autoCompleteShowKey={"alpha3Code"}
    autoCompleteKey={"name"}
    maxTags={5}
    placeholder={"Tags Input..."}
    
		
/>

