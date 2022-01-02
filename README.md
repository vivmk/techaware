# Tech Aware

![image](/static/img/homepage.png)

---

A simple open source Blog to get people closer to technology.

---

- [Contribute](#hello-friend)
  - [Install Hugo](#install-hugo)
  - [Fork this repository](#fork-repo)
  - [Run project locally](#run-locally)
  - [Push to GitHub](#push-to-fork)
  - [Send Pull Request](#pull-request)
  - [License](#license)

## Contribute

See how to make changes and host them to website.

#### [Install Hugo](https://gohugo.io/getting-started/installing/)

#### [Fork this repository](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo)

#### Run project locally:

Clone the repository you forked to your computer:

```bash
$ git clone https://github.com/iamvkm/techaware.git
```

Make changes to the files you want. If you want to create a new post, here is command:

```bash
$ hugo new posts/enter-post-name.md
```

Enter content in post and make the `draft: false` then run these commands to run the project in browser locally:

```bash
$ hugo
$ hugo server
```

#### Push to GitHub:

Add the files in the local repository and stages them for commit:

```bash
git add .
```

Commit the tracked changes and prepares them to be pushed to a remote repository:

```bash
git commit -m "First commit"
```

Push everything to your forked repository:

```bash
git push origin master
```

#### [Send Pull Request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)

## License

Copyright © 2020 Vivek Mishra ([@iamvvekm](https://twitter.com/iamvvekm))

The website is released under the MIT License. Check the [original project license](https://github.com/iamvkm/techaware/blob/master/LICENSE.md) for additional licensing information.
