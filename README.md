# DDM Technology Blog

This is a blog for technologists at DDM.

## Contributing

### Prerequesits

If you're on a Mac there is nothing to install. If you're not using a Mac, you'll need to [install Hugo](https://gohugo.io/getting-started/quick-start/#step-1-install-hugo).

### Write a Post

Here are the commands for creating your blog post.

```
./hugo new posts/my-working-title.md
open ./content/post/my-working-title.md
```

You can rename your post later, just give it a working title to start with.

### Preview Your Post

Once you've started writing you can preview your post locally in the browser. Here's the command.

```
./hugo server -D
```

View it by pointing your browser at http://localhost:1313.

### Publish your Post

To publish your new post, generate the site, commit, and push your changes.

```
./hugo
git commit -m 'my-working-title'
git push
```

We're committing directly to master for now. This reduces the number of steps to get your post published and reduces friction for developers.
