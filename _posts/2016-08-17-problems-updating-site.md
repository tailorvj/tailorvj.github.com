---
published: true
---
## I'm having trouble updating this site at the moment

Update: After managing to finally post new Jekyll posts to the blog, I found the presentation folder repo. It is a separate repo on github with a gh-pages branch for publishing to my github.io site. I completely forgot about this trick because I did this a couple of years ago. To sum things up: subfolders on github.io pages can be published and managed from separate repos where the repo name is the subfolder name and using a gh-pages branch to automatically publish changes to the subfolder. In this specific example I have a repo named "present" in which I hold my presentations and every time I update its' gh-pages branch, tailorvj.github.io/present is updated accordingly. I will commit changes now to the present repo instaed of the tailorvj.github.io repo

Update: Posts are being published using prose.io and Jekyll, but subfolders are not updating. Why?

Update: I got a build warning email saying my Jekyll is using pygments highlighter instead of rouge, so I edited config.yml to fix that. Now editing this post to see if it triggers a site update

This post shouldn't appear at all unless the problem is solved :)

I've added a few presentations from recent lectures and I'm trying to upload them to the site, but after updateing the repository, they won't deploy. I don't know why. After some research into to issue I sent github support an email. 

Now I'm using prose.io in order to post a new Jekyll post to the blog and see whether the blog is updated. Let's see what happens...
