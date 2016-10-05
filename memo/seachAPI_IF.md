* ruby on rails で簡単に作成できそう
* json形式でリクエストして、レスポンスもjson
* jsonの形式についてはもう少し考えます
* いずれかのリクエストパラメータの指定は必要

* リクエストパラメータについて
```json
'schema': {
	'type': 'object',
	'properties': {
		'keyword': {
			'title': 'キーワード',
			'subscrition':'書籍情報のタイトルなど(持つ書籍情報により変わります)、複数の項目を検索する。'
			'type': 'string'
		},
		'title': {
			'title': 'タイトル',
			'subscrition': '書籍のタイトルを検索する'
			'type': 'string'
		},
		'class_number': {
			'title': '分類番号'
			'subscrition': ''
			'type': 'string'
		},
		'author': {
			'title': '著者名'
			'subscrition': ''
			'type': 'string'
		}
	},
}
```

* httpのstatuscodeにAPIのレスポンスに応じたstatus_codeを入れる
* 200:OK,400: BadRequest, 404: Not Found, 500: Internal Server Error ぐらい
* レスポンスパラメータの例
```json
{'num': 2
 'books':[
	{
	'title': 'hoge', 
	'author': 'fuga'…
	}, 
	{
	'title': 'hoge', 
	'author': 'fuga'…
	},
]
}
```
