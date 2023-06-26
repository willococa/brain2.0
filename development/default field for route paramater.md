in the route you can change the default field used as a parameter instead of id to slug (for example)
```
 Route::get('posts/{post:slug}', function (Post $post) { 
    return view('posts.show', compact('post'));
    });
```
you could also instead go to the model and add:
```
    function getRouteKeyName(){
        return 'slug';
    }
```