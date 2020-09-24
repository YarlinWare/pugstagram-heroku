<script context="module">
  export async function preload(){
    let data = {};
    const response = await this.fetch(
      'https://us-central1-pugstagram-co.cloudfunctions.net/data'
    );
    data = await response.json();
    return {data}
  }
</script>
<script>
  // import { onMount} from 'svelte'
  import Main from "../components/Main.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import TimeLine from "../components/TimeLine.svelte";

  // let data = {}
  // const API = "https://us-central1-pugstagram-co.cloudfunctions.net/data"

  // onMount(async ()=>{
  //   const response = await fetch(API);
  //   data = await response.json()
  // })

  export let data;
</script>

<svelte:head>
  <title>Pugstagram</title>
</svelte:head>

<Main>
  <TimeLine posts={data.posts} />
  {#if data.user}
    <Sidebar {...data.user} />
  {/if}
</Main>
