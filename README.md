# DesignStandard

WEB Design Standard，This repository contains the specifications.

Author：Baidu

Collector：Tongjiaqi

## 项目编码规范

来自百度前端团队的前端开发规范，多家国内IT企业共同遵循的开发规范，意在实现项目结构的一致性。

开网科技、本邦科技、中软高科 共同遵循的**项目编码规范**。

* [HTML 编码规范](https://github.com/ecomfe/spec/blob/master/html-style-guide.md)
* [CSS 编码规范](https://github.com/ecomfe/spec/blob/master/css-style-guide.md)
* [JavaScript 编码规范](https://github.com/ecomfe/spec/blob/master/javascript-style-guide.md)

### 自家规范

* [强制] 在 Equality Expression 中使用类型严格的 ===。仅当判断 null 或 undefined 时，允许使用 == null。
```javascript
//正确编写
if(age === 30)
//错误编写
if(age == 30)
//推荐简洁编写
if(!name)
//不推荐编写
if(name == "")
```
* [强制] 调用全局变量前加window.
```javascript
var name = "tongjiaqi";
function log() {
	console.log(window.name);
}
```
* [强制] 单行声明的数组与对象，如果包含元素，{} 和 [] 内紧贴括号部分不允许包含空格
```javascript
var Tomcat = {ip:"192.168.2.2",password:"123"}
var Navicat = [{ip:"192.168.2.2",password:"123"}]
```
