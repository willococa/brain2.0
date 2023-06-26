view composers are used in [[laravel]] to create a variable that you need to always use in an expecific view,  you have to declared them in the appserviceprovider class boot method the like this:
```
class AppServiceProvider extends ServiceProvider
{
    /**
     * Register any application services.
     */
    public function register(): void
    {
        //
    }

    /**
     * Bootstrap any application services.
     */
    public function boot(): void
    {
        \View::composer('users.show', function ($view) {
            $view->with('categories', \App\Models\Category::all());
        });                
    }
}

```

you can do it for all the views by using a wild card (*):
```

        \View::composer('*', function ($view) {
            $view->with('categories', \App\Models\Category::all());
        });
```
or you can instead use the share method:
```
        \View::share("categories", \App\Models\Category::all());                

```
