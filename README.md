### **Node.js仿知乎服务端**

![首页](https://github.com/Monster880/jianshu-react/blob/master/detail.png)
![详情](https://github.com/Monster880/jianshu-react/blob/master/index.png)

#### 1-用户功能开发

- 根据page查找find用户列表
- 通过id查找特定用户findById，在用select选择特定的用户信息
- 实现增加用户的功能，同时实现用户已占用的逻辑
- 实现用户的鉴权checkOwner中间件
- 实现用户的更新update
- 实现用户的删除delete以及用户不存在逻辑的处理
- 实现用户的登录功能login，同时使用jsonwebtoken做权限认证，使用系统变量将用户信息存到ctx.user.state中
- 实现用户的关注功能
- 实现用户的粉丝功能
- 实现用户的关注话题功能
- 实现用户赞答案
- 实现用户踩答案
- 实现用户的Schema设计，与关注的人多对多关系


#### 2-话题功能开发

- 查找话题列表
- 根据id查找话题
- 创建话题
- 更新话题
- 实现话题的Schema设计，与问题的多对多关系


#### 3-问题功能开发

- 查找问题列表
- 根据id查找问题
- 创建问题
- 更新问题
- 实现问题的Schema设计，与话题的多对多关系

#### 4-route模块开发

- 实现了权限认证，检验用户是否存在等中间件
- 使用koa框架，结合githubV3的API实现url的结构
- 使用postman做测试
- postman的url为：https://documenter.getpostman.com/view/11508998/T17Akr6d

#### 5-mongodb数据库连接

### 项目执行 

####  1、将项目克隆到本地，cd到react-jianshu

```javascript
https://github.com/Monster880/koa-restfulapi-zhihu1.git
cd koa-restfulapi-zhihu1
```

#### 2、安装依赖

```javascript
npm install 或 yarn install
```

#### 3、执行

```javascript
npm run dev 或 yarn dev
// (开发环境)
```

以上是参考了Lewis老师的课程制作，并修改了相关的bug