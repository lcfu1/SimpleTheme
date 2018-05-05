# 121

## Theme

- SimpleTheme

  - 采用github主题，和github一样支持Markdown、html等，SimpleTheme只为更好的阅读。
  
  - [使用说明](use/use.md)
  
  - [使用说明](use/use1.md)
  
<h1>2131</h1>

<script>
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