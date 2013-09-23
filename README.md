# organel | 

Organelle responsible for rendering given page template as html. It wraps `jade` template engine to do so.


* `cwd` - Object

  *optional* object containing key:values, where values will be prefixed with `process.cwd()` and placed within config itself with coresponding keys

  Useful to provide `root` value relative to current working directory

* `root` - String

  *optional*, represents the root value to be added in forming page template path.

* `useCache` - false

  Will instruct compiling the template to memory and further use it without any disk IO.

* `page` - String

  *optional*, represents the default page template path to be used if missing in incoming chemicals*/

# incoming | RenderPage

When receiving such chemical the organelle will use it to render the template specified as path within the `page` attribute.  The chemical will be passed as data to the template, so any of its properties will be directly accessible in the template.

* `page` - String
* `root` - String

  *optional*