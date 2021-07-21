<header class='bg-blue-400'>
	<h1>Welcome</h1>
	<nav>
		<a href='/'>Home</a>
		<a href='/about'>About Us</a>
		<a href='/posts'>Posts</a>
	</nav>
</header>

<style lang='scss'>
		//:global(header) {}
    header {
        //background: rebeccapurple;
        color: #fff;
        padding: 20px;
        margin: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

		nav {
			a {
				letter-spacing: 1px;
        color: #fff;
        text-decoration: none;
        padding: 0 10px;
			}
		}
</style>