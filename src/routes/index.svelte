<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
import AddToDiscordBtn from "$lib/AddToDiscordBtn.svelte";

</script>

<svelte:head>
	<title>RadiYo - A Discord Bot for music</title>
</svelte:head>

<section id="hero">
	<div class="col">
		<h1>Music to your server's ears.</h1>
		<p>RadiYo! allows you to listen to internet radio stations in Discord</p>
		<p>✔ 100% free</p>
		<p>✔ Very legal and very cool</p>
		<p>✔ No need to add songs to queue</p>
		<div id="add_btn_holder">
			<AddToDiscordBtn />
			<a href="https://github.com/isiah-lloyd/RadiYo" target="_blank" rel="noopener">
				<img id="github_logo" src="./github.svg" alt="GitHub Logo">
			</a>
		</div>
	</div>
	<div id="hero_img" class="col">
		<img src="./Party.svg" alt="A trio of lads dancing around a disco ball">
	</div>
</section>
<section class="content">
	<!-- svelte-ignore a11y-media-has-caption -->
	<video autoplay muted loop playsinline>
		<source src="./product_demo.webm" type="video/webm" />
	</video>
	<h1>About</h1>
	<p>Unlike those <i>other</i> Discord bots, RadiYo! streams from internet radio stations. This means it is completely legal and will not be shutdown.</p>
	<p>Because RadiYo! streams radio stations, you don't pick and choose each song you want to play. Instead, you find a station that is playing music you like and let their DJ's do the rest.
	   This lets you worry more about your ranked match instead queuing up the next song. RadiYo! includes a feature to search for a station by an artist that's currently playing, this should help you find the right music to fit the mood.</p>
</section>
<section class="content">
	<h1>How to use</h1>
	<p>RadiYo! uses Discord's fancy new <i>slash commands</i>, this means all of RadiYo's commands will autocomplete as soon as you type <i>/radio</i></p>
	<p>Below is a referential list of RadiYo's commands: <br /> (All commands start with /radio)</p>
	<p></p>
	<table>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
		<tr>
			<td>play &lt;query&gt;</td>
			<td>starts a radio station based on your query. try searching by a artist!</td>
		</tr>
		<tr>
			<td>browse</td>
			<td>shows stations we recommend you try! feeling lost? start here!</td>
		</tr>
		<tr>
			<td>asearch &lt;artist&gt; </td>
			<td>search for streams by artist</td>
		</tr>
		<tr>
			<td>gsearch &lt;genre&gt; </td>
			<td>search for streams by genre</td>
		</tr>
		<tr>
			<td>stsearch &lt;station&gt; </td>
			<td>search for streams by station name</td>
		</tr>
		<tr>
			<td>stop</td>
			<td>stops the stream</td>
		</tr>

	</table>

</section>
<section class="content">
	<h1>Support</h1>
	<p>For help, questions, or comments on RadiYo, you can join our <a href="https://discord.gg/aQ4sZ9cJcb" target="_blank" rel="noopener">community Discord server.</a></p>
	<p>If you have found a bug or have a feature request, please <a href="https://github.com/isiah-lloyd/RadiYo/issues/new" rel="noopener">raise an issue in the Github repo</a></p>
</section>
<style>
#hero {
	background-color: #2c2f33;
	display: flex;
	flex-wrap: wrap;
	color: var(--color-white);
	padding-bottom: 2em;
}
.col {
	flex: 50%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
    width: 100%;
	text-align: center;
}
.content {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding: 0 25em;
    text-align: center;
}
#add_btn_holder {
	margin-top: 1.5em;
	display: flex;
	flex-wrap: wrap;
	align-items: center;
}
#github_logo {
	width: 3em;
	margin-left: .3em;
}
.col > * {
	margin: 0.3em;
}
video {
	margin-top: 1em;
	width: 600px;
	height: auto;
}
@media only screen and (max-width: 768px) {
	#hero_img {
		display: none;
	}
	.content {
		padding: 0 0;
	}
	video {
		width: 100%;
	}
}
</style>
