# {{ site.title }}

> Description：{{ site.description }}
>
> author：{{ site.author }}
>
> <a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/subscription" data-show-count="true" aria-label="Watch {{ site.author }}/{{ site.title }} on GitHub">Watch</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}" data-show-count="true" aria-label="Star {{ site.author }}/{{ site.title }} on GitHub">Star</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/fork" data-show-count="true" aria-label="Fork {{ site.author }}/{{ site.title }} on GitHub">Fork</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/issues" data-show-count="true" aria-label="Issue {{ site.author }}/{{ site.title }} on GitHub">Issue</a>
<a class="github-button" href="https://github.com/{{ site.author }}" data-show-count="true" aria-label="Follow @{{ site.author }} on GitHub">Follow @{{ site.author }}</a>
<a class="github-button" href="https://github.com/{{ site.author }}/{{ site.title }}/archive/master.zip" aria-label="Download {{ site.author }}/{{ site.title }} on GitHub">Download</a>

## Theme

- SimpleTheme

  - 采用github主题，和github一样支持Markdown、html等，SimpleTheme只为更好的阅读。
  - [使用说明](use/use.md)
  - [使用说明](use/use1.md)

		<script type="text/javascript">
		Bmob.initialize("d6f5df1e30903a0a49634f3ac9c96ecf", "29bc5d837e8c6054da46fde3ddfce1c8");

		var TestObject = Bmob.Object.extend("{{ site.title }}");
		var testObject = new TestObject();
		testObject.save({
			posts: "{{ page.name }}"
		}, {
			success: function(object) {
				alert("成功");
			},
			error: function(model, error) {
				alert("错误");
			}
		});
		
		var TestObject = Bmob.Object.extend("{{ site.title }}");
		var query = new Bmob.Query(TestObject);
		// 查询所有数据
		query.equalTo("posts", "{{ page.name }}");
		query.find({
			success: function(results) {
				document.getElementById("numb").innerHTML = "阅读   "+results.length;
			},
			error: function(error) {
			}
		});
		</script>