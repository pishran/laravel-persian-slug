# Laravel Persian Slug

ایجاد اسلاگ استاندارد و فارسی در مدل های لاراول

```php
use Illuminate\Database\Eloquent\Model;
use Pishran\LaravelPersianSlug\HasPersianSlug;
use Spatie\Sluggable\SlugOptions;

class Post extends Model
{
    use HasPersianSlug;
    
    public function getSlugOptions(): SlugOptions
    {
        return SlugOptions::create()
            ->generateSlugsFrom('title')
            ->saveSlugsTo('slug');
    }
}
```

اطلاعات بیشتر در مورد کلاس SlugOptions:

https://github.com/spatie/laravel-sluggable#usage

## روش نصب

برای نصب و استفاده از این پکیج می توانید از کامپوزر استفاده کنید:

`composer require pishran/laravel-persian-slug`

## نسخه های قدیمی تر
برای لاوارل ۸ به بعد از آخرین نسخه این پکیج و برای لاراول ۷ از نسخه ۱.۴ استفاده کنید.
