this is a concept in laravel that allows to automatically attach a model to a route
`
```
 Route::get('posts/{post}', function (Post $post) { 
	return view('posts.show', compact('post'));
    });`
```
make sure that the part in the route between brackets has the same name as the variable passed in the function or it wont work