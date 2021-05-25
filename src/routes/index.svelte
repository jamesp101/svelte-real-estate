<script lang="ts">
	import { loremIpsum } from 'lorem-ipsum';
	const header = [
		{
			link: '/',
			title: 'Home'
		},
		{
			link: '/documentation',
			title: 'Hello WOrld'
		},

		{
			link: '/documentation',
			title: 'About us'
		}
	];
</script>

<nav
	class="bg-primary-500
            h-14
            min-h-14
			sticky top-0
		   z-50
            "
>
	<div
		class="text-white
                font-bold
                flex
                float-right
                h-full"
	>
		<div class="my-auto mr-5 antialiased">
			{#each header as h}
				<a href={h.link} class="p-4"> {h.title}</a>
			{/each}
		</div>
	</div>
</nav>

<section class="h-screen w-screen ">
	<div class="h-full w-full absolute select-none -z-1">
		<img
			src="https://images.unsplash.com/photo-1580587771525-78b9dba3b914?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1567&q=80"
			alt=""
			class="h-full w-full object-cover -z-1 select-none"
		/>
	</div>
	<div class="h-full w-full z-50 grid items-center justify-center  z-auto">
		<div class="w-full bg-white rounded-lg p-10 shadow-lg">
			<div class="text-gray-800 font-serif">
				<h1 class="text-5xl font-extrabold">Find Your Place</h1>
				<p>There's no place like <em> home.</em></p>
				<hr class="mt-4 text-gray-900" />
			</div>
			<div class="text-gray-800 font-serif">
				<div class="flex flex-row">
					<div class="flex flex-col m-2 w-full">
						<label for="" class="font-bold">Location</label>
						<input
							type="text"
							name=""
							value=""
							class="w-full rounded-sm"
							placeholder="Enter Address, Street, Zip Code"
						/>
					</div>
				</div>

				<div class="flex flex-row">
					<div class="flex flex-col m-2 w-full">
						<select id="" name="">
							<option value="">For Rent</option>
							<option value="">For Purchase</option>
						</select>
					</div>
				</div>

				<div class="">
					<label for="">Price Range</label>
					<div class="flex flex-row">
						<div class="flex flex-col m-2 w-full">
							<label for="">From</label>
							<input type="number" name="" value="" class="w-full rounded-sm" placeholder="$" />
						</div>

						<div class="flex flex-col m-2 w-full">
							<label for="">To</label>
							<input type="number" name="" value="" class="w-full rounded-sm" placeholder="$" />
						</div>
					</div>
				</div>
			</div>
			<div class="flex flex-row w-full mt-5 font-serif">
				<button
					class="w-full bg-primary-500 py-2 text-white font-bold
								   hover:bg-primary-300 transition "
				>
					Find
				</button>
			</div>
		</div>
	</div>
</section>
<section
	class="h-screen
           w-screen
		   flex font-serif
		   "
>
	<div class="container mx-auto">
		<div class="h-full">
			<h1 class="text-5xl text-gray-800 text-center">Discover Our Best Deals</h1>
			<div
				class="w-full md:w-4/12 lg:w-3/12 border-solid border-2 border-gray-300
					   p-2 rounded-lg"
			>
				<img
					src="https://images.unsplash.com/photo-1570129477492-45c003edd2be?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1050&q=80"
					alt=""
					class="h-20 w-full object-cover"
				/>
			</div>
		</div>
	</div>
</section>
