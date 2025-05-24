---
title: "Why I Chose Hugo (And Ditched Jekyll)"
description: "A quick post on why Hugo made more sense for my blog setup than Jekyll"
date: 2025-05-24T00:47:23+02:00
tags: ["hugo", "blogging", "static-site", "setup"]
author: "Michael Quinton"
draft: false
---

When creating a blog, you’ve got a ton of options. Some are just not as simple as Hugo. Hugo has its downsides, sure—but for me, the pros easily outweigh the cons.

I tried Jekyll at first. The problem? Ruby dependencies. It got annoying fast. I didn’t feel like debugging stuff before I even got to the hard part: actually writing. Weird thing to say as someone in tech, maybe... but I’d rather save the troubleshooting for when it’s really needed.

Sometimes you just want to sit down and put your thoughts into a blog post.

---

### Why Hugo clicked for me

- It’s Go-based, just a single binary
- No install hoops—in my case, just:

```shell
  winget install Hugo.Hugo.Extended
```

It’s minimal, fast, and no-faffing-around. I didn’t need to think too hard.


``` shell
hugo new site blog
cd blog
git init
git submodule add <theme>
hugo new posts/first.md
hugo server
```

Though to be fair, I didn’t use a submodule. I found a theme, cloned it, and started editing it to my liking. Simple as that.

Hugo didn’t get in my way. It let me start writing before getting distracted by systems—and that’s a win in my book.

Now, you might say, "But Jekyll is supported by GitHub Pages." And yeah, it is. GitHub Pages will automatically build Jekyll sites when you push to it, which is definitely a plus.

But with Hugo, you just need to set up a GitHub Actions workflow. Luckily, there are a bunch of prebuilt .yml files out there—or you can roll your own. Here's the official guide:


👉 Deploying Hugo to GitHub Pages