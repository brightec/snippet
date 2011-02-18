Welcome to the snippet module. This allows other modules to define small
pieces of HTML code, snippets, within files. These are then detected
automatically and exposed as blocks within Drupal.

Snippets are ideal for prototyping a site and for static content that
does not change.

To use snippets:

1. Create a 'snippets' directory within your module.

2. Implement hook_snippet_directory() to tell snippets that your module
   contains snippets and where they are (relative to the module directory).

   /**
    * Implements hook_snippet_directory().
    */
   function mymodule_snippet_directory() {
     return 'snippets';
   }

3. Place files in the above directory. These must end in .html. They will
   appear as blocks, and as panel panes.

