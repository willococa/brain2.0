in laravel you can use for 1 days ago format:
```
$post->created_at.diffForHumans();
```

and for Jan, 26, 2018 format
```
$post->created_at->toFormattedDateString();
```

