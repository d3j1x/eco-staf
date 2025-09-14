<script lang="ts">

	import ecostafLogo from '$lib/images/logo-ecostaf.png';


	function closeDrawer() {
		const checkbox = document.getElementById('my-drawer');
		if (checkbox) checkbox.checked = false;
	}
</script>


<div class="navbar bg-base-100 sticky top-0 shadow-sm z-50">
	<div class="navbar-start">
		<a href="/"  class="hidden lg:inline-block"
			><img src={ecostafLogo} class="h-14 rounded-b-xs" alt="ECO STAF Logo" /></a
		>
		<div class="drawer lg:hidden">
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
				class="menu bg-base-200 text-base-content min-h-full w-80 p-4"
			>
				<li><a on:click={closeDrawer} href="/">Acceuil</a></li>
				<li>
					<a on:click={closeDrawer} href="/voitures">Partenaires</a>
					<ul class="p-2 tracking-wider">
						<li><a on:click={closeDrawer} href="/voitures/neuf">Partenaire A</a></li>
						<li><a on:click={closeDrawer} href="/voitures/occasion">Partenaire B</a></li>
					</ul>
				</li>
				<li>
					<a on:click={closeDrawer} href="/services">Services</a>
					<ul class="p-2 tracking-wider">
						<li><a on:click={closeDrawer} href="/services/vidange">Énergie</a></li>
						<li><a on:click={closeDrawer} href="/services/pneu">Télécom</a></li>
						<li><a on:click={closeDrawer} href="/services/freinage">Technologie</a></li>
						
					</ul>
				</li>
				
				<li><a on:click={closeDrawer} href="/localisez-nous">Localisez-nous</a></li>
				<li><a on:click={closeDrawer} href="/aboutUs">À propos</a></li>
			</ul>
	
			</div>
		  </div>
	</div>
		<div class="navbar-center lg:hidden">
		<a href="/" style=""  class=""
			><img src={ecostafLogo} class="h-14 rounded-xs" alt="ECO STAF Logo" /></a
		>
	</div>
	<div class="navbar-center hidden lg:flex">
		<ul class="menu menu-horizontal px-1 text-lg">
			<li><a href="/">Acceuil</a></li>
			<li>
				<details>
					<summary class="px-4"><a href="/voitures">Partenaires</a></summary>
					<ul class="p-2 w-full text-center items-center m-auto">
						<li><a class="text-center m-auto" href="/voitures/neuf">Partenaire A</a></li>
						<li><a class="text-center m-auto" href="/voitures/occasion">Partenaire B</a></li>
					</ul>
				</details>
			</li>

			<li><a href="/services">Énergie</a></li>

			<li><a href="/cartegrise">Télécom</a></li>

			<li><a href="/cpiww">Technologie</a></li>

			<li><a href="/localisez-nous">Localisez-nous</a></li>

			<li><a href="/aboutUs">À propos</a></li>
		</ul>
	</div>
	<div class="navbar-end">

		<input type="checkbox" value="night" class="toggle theme-controller mr-2" />
		
		
	</div>
</div>