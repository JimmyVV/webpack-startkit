
## 安装依赖

npm 版本必须升级到 3.0 +

### 安装fis3

```sh
npm install -g fis3
```
第一步：
### 安装fis3插件

```命令行输入
npm install -g fis-parser-imweb-tpl fis-postprocessor-autoprefixer fis3-deploy-local-deliver fis3-deploy-pack fis3-deploy-skip-packed fis3-hook-annotation fis3-hook-commonjs fis3-hook-lego fis3-parser-node-sass fis3-postpackager-inline fis3-postpackager-loader fis3-prepackager-imweb-ques fis3-hook-node_modules fis3-hook-sys_node_modules fis-parser-babel-6.x fis3-parser-babel fis3-preprocessor-js-require-css fis3-preprocessor-js-require-file
fis-spriter-csssprites-group
```
第二步：
### 安装 `babel` 相关插件

`一定要在父级目录安装插件`

例如 你的目录是 `e:\\fe\\now-app-story`
一定要在 `e:\\fe` 目录执行以下命令

```
tnpm install babel-preset-es2015 babel-preset-es2015-loose babel-preset-stage-0 babel-preset-react
```

### 安装`node_modules`项目资源

项目根目录下运行:

```sh
npm install
```

## 开发

项目根目录下运行:

```sh
npm start
```

## Fiddler / Whistle

### `Fiddler`

- `regex:^https?://your\.domain\.com/(.*\.(js|css|png|jpg|gif|jpeg|svg|blob).*)$` `ROOT:/dev/$1`
- `regex:^https?://your\.domain\.com/[custom path]/([\w\-]*)\.html(.*)$` `ROOT:/dev/pages/$1/index.html`

### `Whistle`

- `/^https?://your\.domain\.com/(.*\.(js|css|png|jpg|gif|jpeg|svg|blob).*)$/` `file:///ROOT:/dev/$1`
- `/^https?://your\.domain\.com/[custom path]/([\w\-]*)\.html(.*)$/` `file:///ROOT:/dev/pages/$1/index.html`

## 发布

```sh
npm run build
```
