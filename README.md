# GitBook Sample

## 手順

```
yarn init
yarn global add gitbook-cli
gitbook --version

yarn gitbook init
gitbook serve
http://localhost:4000/

gitbook build

git add .
git commit -m 'Add GitBook.'
git push -u origin master


git checkout --orphan gh-pages
ls
git checkout master

git subtree push --prefix _book origin gh-pages
```

## 情報追加方法

docs/xxx.md 作成（ここに追加しないとダメ）
SUMMARY.md に追加（追加しないと表示されない）

```
git push origin master
git branch -D gh-pages 
git push origin :gh-pages

git checkout --orphan gh-pages
git checkout master
git subtree push --prefix _book origin gh-pages
```

## わからないこと

### `$ git subtree push --prefix` とは？

### git subtreeでのforceの仕方

`git subtree split --prefix _book master`

[git subtreeで強制的にpushする](https://blog.tk84.net/yKFr/)


## 参考

[GitBookでドキュメントを作ってGithub Pagesで公開する方法 - Casual Developers Note](https://casualdevelopers.com/tech-tips/how-to-publish-gitbook-documents-with-github-pages/)

## Web site URL

https://s4na.github.io/git-book-sample/



https://docs.gitbook.com/

https://qiita.com/arm_band/items/ec5bb0a0d1dec1e6da79
