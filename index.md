---
layout: default
---
<header>
	<h1>{{ site.title }}</h1>
	<p>Etiam quis viverra lorem, in semper lorem. Sed nisl arcu euismod sit amet nisi euismod sed cursus arcu elementum ipsum arcu vivamus quis venenatis orci lorem ipsum et magna feugiat veroeros aliquam. Lorem ipsum dolor sit amet nullam dolore.</p>
</header>

<section class="tiles">

	{% for post in site.posts %}

	<article class="style1">
		<span class="image">
			<img src="{{ post.img }}" alt="{{ post.title }}" />
		</span>
		<a href="{{ post.url }}">
			<h2>{{ post.title }}</h2>
			<div class="content">
				<p>{{ post.excerpt }}</p>
			</div>
		</a>
	</article>

	{% endfor %}

</section>