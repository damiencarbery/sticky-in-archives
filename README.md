# sticky-in-archives
Move sticky posts to top of archive listings.

Read the blog entry at:
http://www.damiencarbery.com/2017/09/sticky-posts-in-category-archives/

By default it operates on all category archives. To limit it to certain categories you can specify them by
using the 'sia_sticky_categories' filter.

```
add_filter( 'sic_sticky_categories', 'pu_set_sticky_categories' );
  function pu_set_sticky_categories( $categories ) {
    // Only operate on these two categories.
	  $categories[] = 'edge-case-2';
	  $categories[] = 'media-2';
	  return $categories;
  }
```

TODO:
- Consider adding support for author or tag archives.
