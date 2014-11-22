redmine2weekly
==============

获取Trello卡片checklist并生成周报发送至指定邮箱

![image](http://ww2.sinaimg.cn/large/6209f836gw1ellihnwa0jj20pw0uo462.jpg)

### 功能特性

- 支持自定义Mailgun账户
- 根据Trello REST API
- 获取Trello卡片中检查表并生成周报展示
- 发送周报到指定收件人

### 本地运行

编辑配置文件
````
$ mv config-example.yml config.yml # 并配置好内容
````
执行bundle install
````
$ [sudo] bundle install
````
执行migration
````
$ [sudo] rake db:migrate
````
执行app.rb
````
$ [sudo] ruby app.rb
````

### Heroku 部署

编辑配置文件
````
$ mv config-example.yml config.yml # 并配置好内容
````
创建heroku app
````
$ [sudo] heroku create your-apps-name
````
提交应用
````
$ [sudo] git push -u heroku master
````
执行migration
````
$ [sudo] heroku rake db:migrate
````

[ ![Codeship Status for xi4oh4o/trello2weekly](https://codeship.com/projects/8eb020e0-c515-0131-98c2-5a1ddad26e1f/status)](https://codeship.com/projects/21996)
