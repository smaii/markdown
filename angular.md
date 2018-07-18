
//全局安装 Angular CLI 
npm install -g @angular/cli(稳定版)  (或angular-cli     =>beta版)

//2. 创建新项目
ng new my-app
ng new my-app --style=scss(sass)使用scss或者sass编译css

//3. 启动开发服务器(进入项目目录)
cd my-app
ng serve --open

ng serve 命令会启动开发服务器，监听文件变化，并在修改这些文件时重新构建此应用。
使用 --open（或 -o）参数可以自动打开浏览器并访问 http://localhost:4200/。
 //4200为默认端口，如果端口被占用，可以重新定义端口。
 ng server --port 4000 -o


利用angular-cli新建一个组件ng g component componentName  (进入component目录)
//新增的组件会自动创建4个文件分别为:name.component.css、name.component.html、name.component.ts、name.component.spec.ts

//删除node_modules文件夹
npm install rimraf -g
rimraf node_modules



//指令

*ngIf , *ngFor ,[class.classNAme]='expression',(click),[ngModel]='value'
//<ng-template [ngIf]>
