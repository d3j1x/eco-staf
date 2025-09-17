<script lang="ts">

	import ecostafLogo from '$lib/images/logo-ecostaf.png';


	function closeDrawer() {
		const checkbox = document.getElementById('my-drawer');
		if (checkbox) checkbox.checked = false;
	}
</script>


<div class="navbar bg-base-100 sticky top-0 shadow-sm z-50">
	<div class="navbar-start">
		<a href="/"  class="hidden md:inline-block"
			><img src={ecostafLogo} class="h-14 rounded-xs -mt-2" alt="ECO STAF Logo" /></a
		>
		<div class="drawer md:hidden">
			<input id="my-drawer" type="checkbox" class="drawer-toggle" />
			<div class="drawer-content">
			  <!-- Page content here -->
			  <label for="my-drawer" class="btn btn-ghost drawer-button">				<svg
				xmlns="http://www.w3.org/2000/svg"
				class="h-8 w-8"
				fill="none"
				viewBox="0 0 24 24"
				stroke="currentColor"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M4 6h16M4 12h8m-8 6h16"
				/>
			</svg></label>
			</div>
			<div class="drawer-side">
			  <label for="my-drawer" aria-label="close sidebar" class="drawer-overlay"></label>
			  <ul
				tabindex="0"
				class="menu bg-gray-100 text-base-content text-blue-600 min-h-full w-80 p-4 font-bold"
			>
				<li><a on:click={closeDrawer} href="/">Acceuil</a></li>
				<li>
					
				</li>
				<li>
					<a on:click={closeDrawer} href="/">Services</a>
					<ul class="p-2 tracking-wider">
						<li><a on:click={closeDrawer} href="/">Énergie</a></li>
						<li><a on:click={closeDrawer} href="/services/telecom">Télécom</a></li>
						<li><a on:click={closeDrawer} href="/">Technologie</a></li>
						
					</ul>
				</li>
				
				<li><a on:click={closeDrawer} href="/locateUS">Localisez-nous</a></li>
				<li><a on:click={closeDrawer} href="/">À propos</a></li>
			</ul>
	
			</div>
		  </div>
	</div>
		<div class="navbar-center md:hidden">
		<a href="/" 
			><img src={ecostafLogo} class="h-14 rounded-xs" alt="ECO STAF Logo" /></a
		>
	</div>
	<div class="navbar-center hidden md:flex">
		<ul class="menu menu-horizontal px-1 text-lg font-bold ">
			<li><a href="/">Acceuil</a></li>

			<li>
				<details>
						<summary class="px-8"><a href="/">Services</a></summary>
						<ul class="py-2 w-full text-center items-center m-auto">
							<li><a class="text-center m-auto" href="/">Énergie</a></li>
							<li><a class="text-center m-auto" href="/services/telecom">Télécom</a></li>
							<li><a class="text-center m-auto" href="/">Technologie</a></li>
						</ul>
				</details>
			</li>




			<li><a href="/locateUS">Localisez-nous</a></li>

			<li><a href="/">À propos</a></li>
		</ul>
	</div>
	<div class="navbar-end">

		<input type="checkbox" value="synthwave" class="toggle theme-controller mr-2" />
		
		
	</div>
</div>