---
---

I added the [Jekyll Redirect Gem](https://github.com/jekyll/jekyll-redirect-from) to account for my old Wordpress permalinks, which didn't have the `html` extension.

I added a customized `_layouts` file called `redirect.html` which includes the `.html` extension if you've enabled it in your config yaml file.

To use, add this variable to the front matter of your note:
```
redirect_from:
  - /free-font-lusitana-by-ana-megda/
  ```
  
You can add multiple old redirect URLs. This plugin generates canonical `link` meta tags pointing to the new note automatically.