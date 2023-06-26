`$posts->with('categories')->get();`

## more than one object

`$posts->with('user','categories')->get();`
## existing object
Now if you already have an object you do it like this
`        $author->posts->load('tags');
## Class level eager loading

` protected $with = ['user', 'categories'];`


