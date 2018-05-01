# DDM Technology Blog

This is a blog for technologists at DDM.

## Contributing

### Prerequesits

If you're on a Mac there is nothing to install. If you're not using a Mac, you'll need to [install Hugo](https://gohugo.io/getting-started/quick-start/#step-1-install-hugo).

### Write a Post

Here are the steps to creating your blog post.

  - Create a new post: `./hugo new posts/my-working-title.md`
  - Edit the file: `open ./content/post/my-working-title.md`

Don't worry, you can rename your post later on. Just give it a working title to start with.

### Preview Your Post

Once you've started writing you can preview your post locally in the browser. Here's how.

  - Run a preview server locally: `./hugo server -D`
  - View it in your browser at http://localhost:1313

### Publish your Post

When you're ready to publish your new post, just commit your changes.

  - Generate the site to the docs folder: `./hugo`
  - Commit your changes: `git commit -m 'my-working-title'`
  - Push your changes: `git push`

We'll commit directly to master for now. This reduces the number of steps you need to take to get your post published and reducing friction may help busy developers post more content.
