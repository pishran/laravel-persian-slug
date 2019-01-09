# Laravel Persian Slug

ایجاد اسلاگ استاندارد و فارسی در مدل های لاراول

```php
use Illuminate\Database\Eloquent\Model;
use Pishran\LaravelPersianSlug\HasPersianSlug;
use Spatie\Sluggable\SlugOptions;

class Post extends Model
{
    public function getSlugOptions(): SlugOptions
    {
        return SlugOptions::create()
            ->generateSlugsFrom('title')
            ->saveSlugsTo('slug');
    }
}
```

## روش نصب

برای نصب و استفاده از این پکیج می توانید از کمپوسر استفاده کنید:

`composer require pishran/laravel-persian-slug`
