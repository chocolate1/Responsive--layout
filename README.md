# 响应式布局
### 随着智能手机的普及，人们获取信息的去到就不仅仅只是从pc端,也从移动端.为了能为不同终端的用户提供更加舒适的界面和更好的用户体验，有了响应式布局--一个网站能够兼容多个终端——而不是为每个终端做一个特定的版本
### 利用@media screen实现网页布局的自适应

### 优点:无需插件和手机主题,对移动设备友好,能够适应各种窗口大小。只需在CSS中添加@media screen属性,根据浏览器宽度判断并输出不同的长宽值
#### 分辨率大于1440
```
@media only screen and (max-width: 1440px) {
    #head, #main{
    width: 100%;
    font-size: 1.2rem;
    }
    .left_text,.left_vedio{
    display: block;
    padding-top: 20px;
    width: 50%;
    float: left;
    margin: 0 auto;
}
.right_text,.right_img{
    padding-top: 20px;
    width: 50%;
    float: left;
    margin: 0 auto;
}
}
```
#### 分辨率大于1340
```
@media only screen and (max-width: 1340px) {
    .right,.left{
        width: 100%;
        height: 400px;
        background-color: orange;
        font-size: 1rem;
        padding-bottom: 10px;
        border-bottom: 1px solid #fff;
    }

}
```
#### 分辨率大于640
```
@media only screen and (max-width: 640px) {
      #head ul{
        width: auto;
        height: 250px;
    }
   #head ul  li{
        width: 100%;
        height: 50px;
        line-height: 50px;
    }
    .left,.right{
        width: 100%;
        display: block;
        height: 500px;
        background-color: pink;
        font-size: .9rem;
        padding-bottom: 1%;
        border-bottom: 1px solid #fff;
    }
    .left_text,.left_vedio,.right_text,.right_img{
    padding-top: 20px;
    width: 100%;
    }
}
```
