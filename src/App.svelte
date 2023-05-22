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
    addKeys={[9]}
    maxTags={5}
    allowPaste={true}
    allowDrop={true}
    splitWith={"/"}
    onlyUnique={false}
    removeKeys={[27]}
    placeholder={"Type Input "}
    
    name={"custom-name"}
    id={"custom-id"}
    allowBlur={true}
    disable={false}
    minChars={3}
		
/>

