---
layout: page
title: "blog"
date: 2013-01-08 11:59
comments: false
sharing: true
footer: true
---

My blog use the [Octopress](http://octopress.org), a blogging framework for hackers. For more infomation, it can be found in its website.

Create new blog
---------------
Blog post
``` sh
rake new_post["title"]
```

Blog page
``` sh
rake new_page[mwiki/blog]
```

Deploy website
--------------
Update in local
``` sh
rake generate
rake preview

```
Then go to the http://localhost:4000 to check the new blogs

Update for online
``` sh
rake setup_github_pages
rake generate
rake deploy
```

Update the source
-----------------
``` sh
git add .
git commit -m 'your message'
git push origin source
```

