<script>
	let name = '';
	let email = '';
	let phoneNumber = '';
	let comment = '';
</script>

<div class="container mx-auto px-4 py-8">
	<h1 class="text-center text-3xl font-bold mb-6 text-white">Contact</h1>
	<p class="text-center text-white mb-6">
		Please fill out the form below and I will get back to you as soon as possible. <br />Form will
		be processed by Formspree.io <br />
	</p>
	<form
		target="_blank"
		action="https://formspree.io/f/xwkgbpnk"
		method="POST"
		class="w-full max-w-lg mx-auto bg-white p-6 shadow-md rounded-lg"
	>
		<div class="mb-4">
			<input
				type="text"
				name="name"
				autocomplete="name"
				class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
				placeholder="Name"
				required
				bind:value={name}
			/>
		</div>
		<div class="mb-4">
			<input
				type="email"
				name="email"
				autocomplete="email"
				class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
				placeholder="Email *"
				required
				bind:value={email}
			/>
		</div>
		<div class="mb-4">
			<input
				type="text"
				name="phoneNumber"
				autocomplete="tel"
				class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
				placeholder="Phone number"
				bind:value={phoneNumber}
			/>
		</div>
		<div class="mb-4">
			<textarea
				name="message"
				placeholder="Comment"
				autocomplete="off"
				class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
				rows="4"
				required
				bind:value={comment}
			></textarea>
		</div>
		<button
			type="submit"
			class="shadow bg-black hover:bg-gray-700 focus:shadow-outline focus:outline-none text-white font-bold py-2 px-4 rounded w-full"
			>Send</button
		>
	</form>
</div>
