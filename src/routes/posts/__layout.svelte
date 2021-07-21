<div class='wrapper'>
	<section>
		<slot />
	</section>
	<aside>
		<h5>Archive</h5>
		<ul>
			<li><a href='/posts'>Posts</a> </li>
			<li><a href='/posts/about'>About posts</a> </li>
			<li><a href='/posts/hello'>Hello post</a> </li>
			<li><a href='/posts/hello-world'>Hello-world post</a> </li>
			<li><a href='/posts/hello/world'>Hello/world post</a> </li>
		</ul>
	</aside>
</div>

<style>
	.wrapper {
			display: flex;
			justify-content: space-between;
			padding: 2rem;
	}

	section {
      padding: .5rem;
	}

	aside {
			background: #f3f3f3;
			width: 25%;
			padding: 1rem;
	}
</style>