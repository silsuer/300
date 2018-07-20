# 《唐诗三百首》数据

```
$ jq .[1] 300.json
{
  "id": 2,
  "contents": "兰叶春葳蕤，桂华秋皎洁。\n欣欣此生意，自尔为佳节。\n谁知林栖者，闻风坐相悦。\n草木有本心，何求美人折？",
  "type": "五言古诗",
  "author": "张九龄",
  "title": "感遇四首之二"
}

$ jq -r '.[] | select(.title == "相思") | .contents + " by " + .author' 300.json
红豆生南国，春来发几枝？
愿君多采撷，此物最相思。 by 王维
```

## 数据来源

http://www.shiku.org/shiku/gs/tangdai.htm
