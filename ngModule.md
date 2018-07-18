

import { ActivatedRoute } from '@angular/router';
//route.snapshot 是一个路由信息的静态快照，抓取自组件刚刚创建完毕之后。
//paramMap 是一个从 URL 中提取的路由参数值的字典。 "id" 对应的值就是要获取的英雄的 id。
  >>ActivatedRoute.snapshot.paramMap.get('id');
  >>ActivatedRoute.snapshot.params['id']


import { Location } from '@angular/common';


import { RouterModule, Routes } from '@angular/router';
	router:Routes = [...]
  >>RouterModule.forRoot(router)


  import { HttpClient, HttpHeaders } from '@angular/common/http';