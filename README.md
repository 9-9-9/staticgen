# StaticGen

[StaticGen.com](http://www.staticgen.com), a leaderboard of top open-source static site generators.

## Contributing

Missing a static site generator here? Just fork the repo and add your generator
as a `<name>.md` in the `source/projects` folder.

Make sure to follow the following rules:

*   **Static Site Generation:** No "flat-file CMSs" or similar tools. The program must be able to output a static website that can be hosted in places like BitBalloon, S3 or Github Pages.
*   **Open Source:** The generator must have a public repository on Github that we can link to and pull in stats from.
*   **Stick to the format:** Fill out all the same fields as the other static site generators in `source/projects`.
*   **Short description:** Keep all the details for the body text, keep the description for the overview page short and sweet.

## Running locally

StaticGen is built with Middleman. To install and run locally:

    git clone https://github.com/BitBalloon/staticgen.git
    cd staticgen
    bundle install
    bundle exec middleman

You'll run into GitHub's API limits very quickly if you just do this. To avoid this we recommend you create a Github API token with permissions to access public repositories and Gist.

Then create a Gist with a single file `data.json` with an empty javascript object literal as content: {}

Then set these environment variables before running middleman:

    export GITHUB_TOKEN=YOUR_TOKEN
    export GIST_ID=ID_OF_YOUR_GIST

Then middleman will use the Gist you specified to archive stats (stars, forks and issues) for the repositories.

## BitBalloon

StaticGen is built and maintained by [BitBalloon](https://www.bitballoon.com), a hosting service for static websites.

## License
This project is licensed under the [MIT license](http://opensource.org/licenses/MIT).

StaticGen
StaticGen.com，顶级开源静态站点生成一个排行榜。

特约

缺少一个静态的网站发生器在这里？刚叉回购，并添加您的发电机为<名>.md源/项目的文件夹中。

请务必遵循以下规则：

静态网站生成：无“平面文件的CMS”或类似的工具。该程序必须能够输出一个静态网站，可以在像BitBalloon，S3或Github上页的地方举办。
开源：发电机必须有一个公共仓库Github上，我们可以链接到拉从统计数据。
坚持格式：填写所有相同的字段作为其他静态网站生成源/项目。
简短说明：保留所有的细节正文，保持了概述页面简短而亲切的说明。
本地运行

StaticGen是建立与中间人。要安装和运行在本地：

混帐克隆https://github.com/BitBalloon/staticgen.git
CD staticgen
安装捆绑包
束EXEC中间人
你会碰到GitHub的API限制速度非常快，如果你只是这样做。为了避免这种情况，我们建议您创建权限访问公共库和要点的Github上API令牌。

然后创建一个文件data.json一个空的JavaScript对象文字作为内容的要点是：{}

然后设置运行中间人之前这些环境变量：

出口GITHUB_TOKEN= YOUR_TOKEN
出口GIST_ID= ID_OF_YOUR_GIST
然后，中间人将使用您指定的存档统计（星星，叉和问题）的仓库的要点。

BitBalloon

StaticGen是建立和BitBalloon，静态网站托管服务维护。

许可证

该项目是根据MIT许可证授权。
