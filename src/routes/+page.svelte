<script lang="ts">
	import Router from 'svelte-spa-router';
	import WalletManager from '../components/wallet/WalletManager.svelte';
	import NetworkManager from '../components/network/NetworkManager.svelte';
	import SmartContractManager from '../components/contract/SmartContractManager.svelte';
	import ScheduleManager from '../components/schedule/ScheduleManager.svelte';
	import TokenManager from '../components/token/TokenManager.svelte';
</script>

<div class="container">
	<Router
		routes={{
			'/': ScheduleManager,
			'/wallet': WalletManager,
			'/network': NetworkManager,
			'/token': TokenManager,
			'/contract': SmartContractManager
		}}
	/>
</div>
