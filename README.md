# theme-test

Testing the use of a custom gh-pages theme. 

This is the minimum set of files needed to import and apply a remote theme. 

```
markdown: kramdown
remote_theme: mmistakes/minimal-mistakes
```

index.md, _config.yml, and assets/images copied from the starter template: 

https://github.com/lecy/mmistakes-test

Which was a template repo that contains example site content files the user can easily customize: 

https://github.com/mmistakes/mm-github-pages-starter

The theme design/style elements are all stored in the theme repo:

https://github.com/mmistakes/minimal-mistakes

If you want multiple projects to use the same theme it is suggested to create a gem-based theme and a starter template like above. 

The advantage is that updates to the theme will automatically propogate to all of the project pages using the remote theme. 

## Updates to Themes

When you are using a remote_theme then changes made by the developer to the underlying theme should propogate to your site. 

Any files you create that have identical names as files in the original theme will replace the theme files. 

This allows you to extend the original theme by customizing the design elements (includes, layout, CSS, etc.). When you add a file to your local repo it takes precedence over the original theme file and will replace it. 

Take care, though, to not accidentally replace elements that [prevent you from receiving updates to your theme](https://jekyllrb.com/docs/themes/): 

*Note that making copies of theme files will prevent you from receiving any theme updates on those files. An alternative, to continue getting theme updates on all stylesheets, is to use higher specificity CSS selectors in your own additional, originally named CSS files.*
