<script context="module">
	// loading before page loads
	// type LoadInput ={
	// 	page: {
	// 	host: string;
	// 	path: string;
	// 	params: Record<string, string | string[]>;
	// 	query: URLSearchParams;
	// 	};
	// 	fetch: (info: RequestInfo, init?: RequestInit) => Promise<Response>;
	// 	session: any;
	// 	context: Record<string, any>;
	// };
	//
	// type LoadOutput = {
	// 	status?: number;
	// 	error?: Error;
	// 	redirect?: string;
	// 	props?: Record<string, any>;
	// 	context?: Record<string, any>;
	// 	maxage?: number;
	// };
	export async function load({ page }) {
		const Hello = (await import(`../../posts/${page.params.slug}.md`));

		const post = {
			title: page.params.slug,
			date: new Date(),
			body: 'Lorem ipsum...'
		};

		return {
			props: {
				Hello: Hello,
				title: Hello.metadata.title,
				 // post
			}
		}
	}
</script>

<script>
	// import Hello from '../../posts/hello.md';

	// export let post;
	export let Hello;
	export let title;
</script>

<h2>{title}</h2>
<Hello />