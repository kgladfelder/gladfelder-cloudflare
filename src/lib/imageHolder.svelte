<script lang="ts">
	export let image: string;
	export let desc: string;
</script>

<main>
	<enhanced:img alt={desc} src={image} />
    <h5>{desc}</h5>
</main>

<style>
    @font-face {
        font-family: 'Gelasio';
        font-style: normal;
        font-weight: 400;
        src: local('Gelasio Regular'), local('Gelasio-Regular'), url(https://fonts.gstatic.com/s/gelasio/v1/cIf9MaFfvUQxTTqS9C6hYQ.woff2) format('woff2');
        unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
    }
	img {
		width: 45vw;
		height: auto;
		margin-left: auto;
		margin-right: auto;
		display: block;
        padding-top: 1em;
	}

    @media (max-width: 800px) {
		img {
			width: 90vw;
		}
	}
    h5 {
        margin-left: 2em;
        font-family: Gelasio;
    }
</style>
