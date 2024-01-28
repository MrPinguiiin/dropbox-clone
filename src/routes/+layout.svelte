<script lang="ts">

import Header from "$lib/components/Header.svelte";
import { ModeWatcher } from "mode-watcher";
// import Footer from "$lib/components/Footer.svelte";

import "../app.pcss";

</script>

<Header />
<ModeWatcher />
<slot />