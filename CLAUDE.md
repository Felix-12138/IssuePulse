# CLAUDE.md

项目目标：用户提交反馈，PM 筛选/标记优先级并生成周报。
技术栈：Node.js+Express，vanilla HTML/CSS/JS，JSON 文件存储，零构建。
约定：数据 {id,title,content,submitter,priority(h/m/l),status(o/p/r),ts}；API 统一 {success,data/error}；状态 open→prioritized→resolved。
命令：`npm install` / `npm start`（3000 端口）。
编码：新增枚举须同步前后端；JSON 原子写入（tmp→rename）；data/ 不提交。
验收：三页面全流程通畅，覆盖加载/空/错误/成功状态，JSON 损坏不崩溃。
禁止：不加构建/框架/认证；不改 git config。

使用该项目的用户是一个AI产品经理，没有代码开发经验，所以你写的代码要尽量简洁、易懂，关键代码段一定要添加注释。