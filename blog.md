2016.7.4
=============
- 給 linux-mint USB-DISK 安裝 git、拼音輸入法
- 參考 pages.github.com，建設個人網頁

to - do:
- 參考 blog.fens.me 上面的 node.js 入門系列，學習 node.js 的使用
- 了解 electron，學習使用其開發應用


2016.7.5
=============
- install sublime, node.js

    curl -O https://nodejs.org/dist/v4.4.7/node-v4.4.7-linux-x64.tar.xz
    tar xf node-v4.4.7-linux-x64.tar.xz
    mv node-v4.4.7-linux-x64 ~/bin/
    ln -s ~/bin/node-v4.4.7-linux-x64/bin/node ~/bin/node
    ln -s ~/bin/node-v4.4.7-linux-x64/bin/npm ~/bin/npm

- learning node.js

    - http://www.nodebeginner.org/index-zh-cn.html
    - http://debuggable.com/posts/understanding-node-js:4bd98440-45e4-4a9a-8ef7-0f7ecbdd56cb
    - https://howtonode.org/deploy-blog-to-heroku

- sign up to heroku.com with my email at live.com for node testing
- install Heroku client ( https://toolbelt.heroku.com/ )

2016.7.6
=============
- install chrome

    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
    sudo dpkg -i google-chrome-stable_current_amd64.deb
    sudo apt -f install

- learning node.js from https://howtonode.org/deploy-blog-to-heroku

- learning how to deploy projects to heroku from https://devcenter.heroku.com/articles/getting-started-with-nodejs

	# 獲取初始項目資源
    git clone https://github.com/heroku/node-js-getting-started.git
	cd node-js-getting-started

	# 在 heroku 上新建 app
	heroku create

	# 將本地項目資源上傳 heroku
	git push heroku master

	# 讓 heroku 至少運行一個實例
    heroku ps:scale web=1

	# 打開網頁看看效果
	heroku open [url]

	# 看看日志
	heroku log --tail
2016.7.7
===========
continue learning heroku:

    # create a sample package.json file
    npm init --yes

    # install the app dependencies locally
    npm install

    # run the app locally
    heroku local web

    # add another package
    npm install --save --save-exact same-package

    # push local changes
    git add .
    git commit -m "blablabla..."
    git push heroku master

2016.7.11
============
install VPN client with GUI

  $ sudo apt install network-manager-pptp network-manager-pptp-gnome network-manager-openvpn network-manager-openvpn-gnome
