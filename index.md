---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
<main>
  <style>
  ul { list-style: none;
       padding-left: 0; 
  }
  </style>
  <ul>
    {% for post in site.posts %}
      <li>
        <h1>  
		  <a href="{{ post.url }}">
            {{ post.title }}
          </a>
		</h1>
        <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
		<hr>
	    <p>
	      {{ post.content }}
		</p>
      </li>
    {% endfor %}
  </ul>
</main>

###### What is the purpose of this page, this website, the Internet, and the digital world as a whole?





















