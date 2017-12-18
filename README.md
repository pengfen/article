github.com 创建 article项目-**

cd /g/article
git init
git remote add origin git@github.com:pengfen/article.git
git pull origin master
echo '' >> README.md
git add README.md
git commit -m f
git push origin master

http://npm.taobao.org/
alias cnpm="npm --registry=https://registry.npm.taobao.org \
--cache=$HOME/.npm/.cache/cnpm \
--disturl=https://npm.taobao.org/dist \
--userconfig=$HOME/.cnpmrc"

cnpm -v
cnpm install vue-cli -g
vue init webpack article-ui #文章前端 (使用vue2.js)
install vue-router #选择 yes

cd article-ui
cnpm install
cnpm run dev

localhost:8080