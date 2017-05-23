# sync-post-types-to-taxonomies
A WordPress plugin providing an API for plugin developers to sync specified a post type with a specified taxonomy, multiple pairs of post types and taxonomies can be synced.

# Instructions
Drop the file inside `wp-content/plugins/` and create connections between your post types and taxonomies like so:

```
  add_filter( 'sptt_sync', function( $sync_with ) {
    $sync_with['post_type_slug'] = 'taxonomy_slug';
    return $sync_with;
  });
```
