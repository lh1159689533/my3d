# my3d

使用es6写的3d组件

## 安装
`npm install git+https://github.com/lh1159689533/my3d.git --save`

## 引入
`import Obj3d from "@liuh/my3d"`

## 使用
```
1.创建墙
let wall = Obj3d.create({
	name: "wall-front",
	type: "wall",
	size: [28.2, 1.6, 0.2],
	position: [0, -7.5, 0.8],
	frames: [
	{
	  size: [1, 1, 0.2],
	  position: [-12, -7.5, 0.8],
	},
	{
	  size: [1, 1, 0.2],
	  position: [12, -7.5, 0.8],
	},
	]
});
2.拷贝墙
Obj3d.clone(wall, {
	name: "wall-right",
	position: [-14, 0, 0.8],
});
```
