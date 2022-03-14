## The difference between `git pull` and `git fetch`

## Let's start with a primer on both commands

How would you evaluate the usage of those commands if you were tasked to do some commits in a team?

Which of those commands is more _destructive_ than the other?

Read on to discover and if you enjoyed this article, leave a _like_ or a _unicorn_ or whatever makes you happier and it will surely make me happy aswell!

Also, you can find similar blogposts in my main blog [404answernotfound.eu](https://404answernotfound.eu) where I write about **technology, innovation, programming and most importantly, memes**.


![Git pull and star wars](https://cdn.hashnode.com/res/hashnode/image/upload/v1646817965959/RSuqRY6cb.jpeg)

## `git pull`

In it's simplest usage, `git pull` just wants you to be happy and up-to-date with whatever changes occurred to the remote repository. _Any changes_, _anything at all_ will be **pulled** from the remote repo and automatically _merged_ into your cloned local repository.

See where I'm getting at? It can be problematic, especially the automatic part.

## `git fetch`

To make sure that we are up-to-date with remote changes but without the fear of destroying the subtle existence of our local changes we can do `git fetch` which will (you guessed it!) _fetch_ any commits that were done remotely and do not exist on your local repo, keeping you repo up-to-date **without** merging the new changes with your current branch, making it safer to update without worrying too much about disruption brought by merging conflicts and so on.

## The difference between pull and fetch

So, what's the big time difference between those two commands? Usage and timing.


![git pull or git fetch](https://cdn.hashnode.com/res/hashnode/image/upload/v1646818291522/WC3QyJYW_.jpeg)

 `git pull` actually does a `git fetch` followed by a `git merge`, so, if you just want to keep your repository updated while working on your own local commits, make sure you do a lot of `git fetch(es)` to avoid changes in your `refs/heads` (where you are working) but still keeping your  `refs/remotes` up-to-date.

## Goodbyes

I hope you enjoyed this content and found it useful for your daily activities at work or for your hobbies. If you have any requests, drop a message on one of my social media accounts or open an issue/start a discussion on github, on this [repository](https://github.com/404answernotfound/community/discussions)!

As always you can find me on [Twitter](https://twitter.com/404answnotfound), listen to my [Podcast on Spotify](https://open.spotify.com/show/0d3hBsVITjcFRxPRqvNtCQ?si=e060235591d54152) and add me on [LinkedIn](https://www.linkedin.com/in/lorenzopieri/) to talk professionally (_yeah, right_!)
