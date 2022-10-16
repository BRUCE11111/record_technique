## Install

## windows

### Nodejs

Firstly, you should download Node.js.

[Node.js (nodejs.org)](https://nodejs.org/en/)

Remember install the `LTS` version. I install the 64bit package. All of the install options select default, you just need to click `next`.

When the installation is complete, you can press `Win+R` to open the command prompt and enter `node -v` and `npm -v`. If the version number appears, the installation is successful.

> If you do not have a ladder, you can use Alibaba's domestic mirror for acceleration.

```bash
npm config set registry https://registry.npm.taobao.org
```

### Git

Install git. You can search it in google.

### Install hexo

Create a new folder in a suitable place to store your blog files. For example, my blog files are stored in the `D:\1\blog`.

Open your command prompt and input `npm i hexo-cli -g` to install hexo.

If you get a few errors. Just ignore it.

After complect the installation, enter `hexo -v` to verify the installation.

Then we need to initialize our website by typing `hexo init` to initialize the folder. Then enter `npm install` install the necessary components.

Type `hexo g` to create a static web page. Then type `hexo s` to open the local server. Then open your brower to `http://localhost:4000/` and you'll see our blog.

Entering `ctrl c` to close local server.

### Back up blog's files

If we want to write the blog on another computer, we can upload all the blog files to github.

Firstly, create a branch called `hexo` in the github blog repository, then `git clone` to local pc, take out the .git folder, and place it in the root directory of your blog.

Then entering `git branch -b hexo` to change to `hexo` branch. Entering `git add .` ,`git commit -m 'xxx'` and `git push origin hexo` to submit to github.

### Writing article

Right-clicking in your blog root directory to open command prompt and enter `hexo new post "xxx"` to create a new article.

Then open `source\post`directory, you can find a folder and a.md file below, one is used to store your pictures and other data, the other is your post file.

After writing the mardkown files, type `hexo g` in the root directory to generate a static web page, then type `hexo s` to preview the website locally, and finally type `hexo d` to upload it to github. Open your `github.io` page and you'll see the post.



