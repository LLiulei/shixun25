### 总结12.25号的内容
---

## 开发流程

    1、需求评审(项目负责人，老板，产品经理，技术总监)
    2、技术评审(前后端开发人员、UI测试)，原型图已出(比较粗糙)
    3、排期，让后端先估时间，在产品经理能接受的情况下，尽量估长一点(定接口时间+开发时间+联调时间)
    4、设计先启动，前端和后端等待
    5、开发阶段:定接口，独立开发联调
    6、提交测试，先把文件上传到服务器上(git自动化或者ftp文件服务器),拼接成一个路径形式:发送邮件给测试,里面包含测试地址和一些说明
    7、测试通过，发布上线，一般在晚上在公司等着就好，风险大多在服务端，我们只需要把线上地址发出来

## 项目规范

    代码规范: 工程目录结构，编码分格(ESLint)
    代码管理规范: Svn、Git分支管理，每人一个分支，开发完成提交pull request
    仓库管理: gitlab(完全免费的开源软件，按照MIT许可证分发),coding(是一个面向开发者的云端开发平台，目前提供代码托管，运行空间，质量控制，项目管理等功能),gitee(中国版的github),github(国外的)
    发布规范: 成熟的发布系统，CI系统，自动化部署

## 项目沟通

    需求方: 产品经理，一定会不断改需求的，这时候我们要保留好与其沟通的证据;先答应下来，然后不做
    后端: 定好接口就行，沟通好排期，什么时候测试什么时候联调
    沟通工具: 钉钉

## 项目人员构成(20个)

    技术负责人/项目总监/技术总监/CTO(1个): 技术选型 把控整个项目
    需求方(3个): 产品经理(2个)、运营人员(1个)
    开发人员(16个): UI设计(2个)、前端开发(4个)、后端开发(7个)、测试人员(2个)、运维人员(负责上线，配置线上环境) (1个)
    记住一点就行: 你说的都对

## 接口的组成

    接口的作用
    传过去的参数
    接口的返回值: code: 状态码
                 data: 业务数据
                 msg: 错误提示信息，由后端返回，前端一般直接提示即可