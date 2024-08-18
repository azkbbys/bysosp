# 岛三速建

## 文档说明

本文档中的代码，如果出现“-snip-”表示省略了上文中重复的代码

## 建筑代码

### 岛三的建筑代码

voxels.setVoxel()可以指定最多5个参数：X, Y, Z, voxel, rotation

#### 限制

参数X, Y, Z必须是string；voxel, rotation可以是string或者number类型

```javascript
voxels.setVoxel(X, Y, Z, voxel, rotation)
/*
(x: number, y: number, Z: number, voxel: string | number, rotation?: string | number) : number
*/
```

### 举例

如 `voxels.setVoxel(1, 1, 1, 'grass', 0)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为0即方块旋转0*90=0度

如 `voxels.setVoxel(1, 1, 1, 'grass', 1)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为1即将方块逆时针旋转1*90=90度

又如 `voxels.setVoxel(1, 2, 3, 'stone', 2)`，可以在x=1,y=2,z=3的位置放置一个石头，因为旋转（rotation）的值为2，所以会将原始的方块逆时针旋转2*90=180度

`voxels.setVoxel(12, 3, 45, 'glass', 3)`，在x=12,y=3,z=45的位置放置一个玻璃方块，逆时针旋转3*90=270度

`voxels.setVoxel(12, 3, 45, 'dirt', 4)`，在x=12,y=3,z=45的位置放置一个土方块，逆时针旋转了4*90=360度，所以相当于不旋转，作用效果等于 `voxels.setVoxel(12, 3, 45, 'dirt', 0)`

说明：rotation值可以不加，默认为0

### 返回值

#### 方块存在时

如果传入的方块存在，使用此方法的返回值会返回第四个参数即voxel对应的方块ID

例如 `voxels.setVoxel(1, 2, 3, 'stone')`会返回名为“stone”的方块对应的id

#### 方块不存在时

如果方块不存在，会返回0

例如 `voxels.setVoxel(1, 2, 3, 'this_is_not_a_block_name')`会返回0

## 快速建造

快速建造可以更高效地批量化建筑方块

### 建造一个长方体

```javascript
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}
```

#### 举例

```javascript
// 定义函数
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}

// 调用函数
// 调用快速建造函数用“grass”（草方块）建造一个起于{x=1,y=1,z=1}，止于{x=100,y=64,z=101}，所有方块都旋转3*90=270度的长方体
quick_build('grass', 1, 1, 1, 100, 64, 101, 3)
// 调用快速建造函数用“stone”（草方块）建造一个起于{x=2,y=3,z=4}，止于{x=100,y=64,z=101}，此时不传入参数rotation，方块默认不旋转
quick_build('stone', 2, 3, 4, 100, 64, 101, 3)
```

#### 解决分不清x,y,z的最大值和最小值的问题

有时候并不知道xmin,ymin,zmin,xmax,ymax,zmax到底该传入什么值，以下两种方法可以解决：

##### 如果已经知道定值，可以自行判断

例如：

```javascript
var pos1 = new GameVector3(1,1,1)
var pos2 = new GameVector3(5,5,5)
```

因为pos1的x、y、z值都小于pos2的x、y、z值，所以此时应如此传入：

```javascript
quick_build('方块名', pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos3.z)
```

##### 如果两坐标完全随机，可以使用函数判断

```javascript
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	-snip-
}
function quick_build_pro(voxel, pos1, pos2, rotation=0){
	// 判断pos1和pos2的位置关系并正确传入
	if(pos1.x<=pos2.x&&pos1.y<=pos2.y&&pos1.z<=pos2.z){ // 当pos1的xyz坐标均小于等于pos2的xyz坐标时的调用方式
		quick_build(voxel, pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos2.z, rotation)
	}
	else if(pos1.x>pos2.x&&pos1.y>pos2.y&&pos1.z>pos2.z){ // 当pos2的xyz坐标均小于pos1的xyz坐标时的调用方式
		quick_build(voxel, pos2.x, pos2.y, pos2.z, pos1.x, pos1.y, pos1.z, rotation)
	}
	else{ // 否则输出错误
		console.error('不支持的判断类型')
	}
}
```

### 以某一位置为中心建造球体

```javascript
/**
 * 快速建造一个球体
 * 
 * @param {GameVector3} centerPos - 球体中心位置
 * @param {number | string} voxel - 方块id或名称
 * @param {number} r - 球体半径
 * @param {number | string} rotation - 方块旋转
*/
function ball(centerPos, r, voxel, rotation=0){
	// 创建嵌套循环，这样创建的妙处在于不必遍历地图每个方块，如果遍历地图每个方块的话地图会崩溃
	for(let x=centerPos.x-r;x<=centerPos.x+r;x++){
		for(let y=centerPos.y-r;y<=centerPos.y+r;y++){
		for(let z=centerPos.z-r;z<=centerPos.z+r;z++){
        	const position2 = new GameVector3(x, y, z);

                // 计算两个位置之间的距离
                const distance1 = Math.sqrt(Math.pow(position2.x - centerPos.x, 2) + Math.pow(position2.y - centerPos.y, 2) + Math.pow(position2.z - centerPos.z, 2));
          	if(distance1<=r){// 如果距离小于传入的r的值，则放置方块
                     	voxels.setVoxel(x,y,z,voxel,rotation)
            	}
                }
            	}
     	}
}
```

#### 限制

因为神奇代码岛的服务器能力问题，当r过大时可能会导致服务器崩溃，所以不要传入一个较大的值

#### 举例

```javascript
function ball(centerPos, r, voxel, rotation=0){
	-snip-
}

var center = new GameVector3(50, 50, 50)
ball(center, 10, 'dirt', 2) // 以{x=50,y=50,z=50}为球体中心、填充旋转了2*90=180度的“dirt”（草方块），半径为10，快速建造一个球体
```

### 在某一位置创建底面为l，高为l的三棱锥

```javascript
function pyramid(l, pos, voxel, rotation){
	let cx = pos.x;
	let cy = pos.y;
	let cz = pos.z;
	let height = l;
	let xend = cx + l;
	let zend = cz + l;
	for(let y = cy; y < cy + height; y++){
	  	let ylevel = y - cy;
	  	let xstart = cx + ylevel;
	  	let xend = cx + l - ylevel;
	  	let zstart = cz + ylevel;
	  	let zend = cz + l - ylevel;
	  	for(let x = xstart; x < xend; x++){
	    	for(let z = zstart; z < zend; z++){
	      		voxels.setVoxel(x, y, z, voxel, rotation);
	    	}
	  	}
	}
}
```

#### 举例

```javascript
function pyramid(l, pos, voxel, rotation){
	-snip-
}
var pos = new GameVector3(60,10,60)
pyramid(5, pos, 'stone', 3); // 在{x:60,y:10,z:60}使用“stone”（石头）建造一个底面为5*5，高度为5的三棱锥，所有方块逆时针旋转3*90=270度
```
=======
<<<<<<< HEAD
# 岛三速建

## 文档说明

本文档中的代码，如果出现“-snip-”表示省略了上文中重复的代码

## 建筑代码

### 岛三的建筑代码

voxels.setVoxel()可以指定最多5个参数：X, Y, Z, voxel, rotation

#### 限制

参数X, Y, Z必须是string；voxel, rotation可以是string或者number类型

```javascript
voxels.setVoxel(X, Y, Z, voxel, rotation)
/*
(x: number, y: number, Z: number, voxel: string | number, rotation?: string | number) : number
*/
```

### 举例

如 `voxels.setVoxel(1, 1, 1, 'grass', 0)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为0即方块旋转0*90=0度

如 `voxels.setVoxel(1, 1, 1, 'grass', 1)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为1即将方块逆时针旋转1*90=90度

又如 `voxels.setVoxel(1, 2, 3, 'stone', 2)`，可以在x=1,y=2,z=3的位置放置一个石头，因为旋转（rotation）的值为2，所以会将原始的方块逆时针旋转2*90=180度

`voxels.setVoxel(12, 3, 45, 'glass', 3)`，在x=12,y=3,z=45的位置放置一个玻璃方块，逆时针旋转3*90=270度

`voxels.setVoxel(12, 3, 45, 'dirt', 4)`，在x=12,y=3,z=45的位置放置一个土方块，逆时针旋转了4*90=360度，所以相当于不旋转，作用效果等于 `voxels.setVoxel(12, 3, 45, 'dirt', 0)`

说明：rotation值可以不加，默认为0

### 返回值

#### 方块存在时

如果传入的方块存在，使用此方法的返回值会返回第四个参数即voxel对应的方块ID

例如 `voxels.setVoxel(1, 2, 3, 'stone')`会返回名为“stone”的方块对应的id

#### 方块不存在时

如果方块不存在，会返回0

例如 `voxels.setVoxel(1, 2, 3, 'this_is_not_a_block_name')`会返回0

## 快速建造

快速建造可以更高效地批量化建筑方块

### 建造一个长方体

```javascript
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}
```

#### 举例

```javascript
// 定义函数
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}

// 调用函数
// 调用快速建造函数用“grass”（草方块）建造一个起于{x=1,y=1,z=1}，止于{x=100,y=64,z=101}，所有方块都旋转3*90=270度的长方体
quick_build('grass', 1, 1, 1, 100, 64, 101, 3)
// 调用快速建造函数用“stone”（草方块）建造一个起于{x=2,y=3,z=4}，止于{x=100,y=64,z=101}，此时不传入参数rotation，方块默认不旋转
quick_build('stone', 2, 3, 4, 100, 64, 101, 3)
```

#### 解决分不清x,y,z的最大值和最小值的问题

有时候并不知道xmin,ymin,zmin,xmax,ymax,zmax到底该传入什么值，以下两种方法可以解决：

##### 如果已经知道定值，可以自行判断

例如：

```javascript
var pos1 = new GameVector3(1,1,1)
var pos2 = new GameVector3(5,5,5)
```

因为pos1的x、y、z值都小于pos2的x、y、z值，所以此时应如此传入：

```javascript
quick_build('方块名', pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos3.z)
```

##### 如果两坐标完全随机，可以使用函数判断

```javascript
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	-snip-
}
function quick_build_pro(voxel, pos1, pos2, rotation=0){
	// 判断pos1和pos2的位置关系并正确传入
	if(pos1.x<=pos2.x&&pos1.y<=pos2.y&&pos1.z<=pos2.z){ // 当pos1的xyz坐标均小于等于pos2的xyz坐标时的调用方式
		quick_build(voxel, pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos2.z, rotation)
	}
	else if(pos1.x>pos2.x&&pos1.y>pos2.y&&pos1.z>pos2.z){ // 当pos2的xyz坐标均小于pos1的xyz坐标时的调用方式
		quick_build(voxel, pos2.x, pos2.y, pos2.z, pos1.x, pos1.y, pos1.z, rotation)
	}
	else{ // 否则输出错误
		console.error('不支持的判断类型')
	}
}
```

### 以某一位置为中心建造球体

```javascript
/**
 * 快速建造一个球体
 * 
 * @param {GameVector3} centerPos - 球体中心位置
 * @param {number | string} voxel - 方块id或名称
 * @param {number} r - 球体半径
 * @param {number | string} rotation - 方块旋转
*/
function ball(centerPos, r, voxel, rotation=0){
	// 创建嵌套循环，这样创建的妙处在于不必遍历地图每个方块，如果遍历地图每个方块的话地图会崩溃
	for(let x=centerPos.x-r;x<=centerPos.x+r;x++){
		for(let y=centerPos.y-r;y<=centerPos.y+r;y++){
		for(let z=centerPos.z-r;z<=centerPos.z+r;z++){
        	const position2 = new GameVector3(x, y, z);

                // 计算两个位置之间的距离
                const distance1 = Math.sqrt(Math.pow(position2.x - centerPos.x, 2) + Math.pow(position2.y - centerPos.y, 2) + Math.pow(position2.z - centerPos.z, 2));
          	if(distance1<=r){// 如果距离小于传入的r的值，则放置方块
                     	voxels.setVoxel(x,y,z,voxel,rotation)
            	}
                }
            	}
     	}
}
```

#### 限制

因为神奇代码岛的服务器能力问题，当r过大时可能会导致服务器崩溃，所以不要传入一个较大的值

#### 举例

```javascript
function ball(centerPos, r, voxel, rotation=0){
	-snip-
}

var center = new GameVector3(50, 50, 50)
ball(center, 10, 'dirt', 2) // 以{x=50,y=50,z=50}为球体中心、填充旋转了2*90=180度的“dirt”（草方块），半径为10，快速建造一个球体
```

### 在某一位置创建底面为l，高为l的三棱锥

```javascript
function pyramid(l, pos, voxel, rotation){
	let cx = pos.x;
	let cy = pos.y;
	let cz = pos.z;
	let height = l;
	let xend = cx + l;
	let zend = cz + l;
	for(let y = cy; y < cy + height; y++){
	  	let ylevel = y - cy;
	  	let xstart = cx + ylevel;
	  	let xend = cx + l - ylevel;
	  	let zstart = cz + ylevel;
	  	let zend = cz + l - ylevel;
	  	for(let x = xstart; x < xend; x++){
	    	for(let z = zstart; z < zend; z++){
	      		voxels.setVoxel(x, y, z, voxel, rotation);
	    	}
	  	}
	}
}
```

#### 举例

```javascript
function pyramid(l, pos, voxel, rotation){
	-snip-
}
var pos = new GameVector3(60,10,60)
pyramid(5, pos, 'stone', 3); // 在{x:60,y:10,z:60}使用“stone”（石头）建造一个底面为5*5，高度为5的三棱锥，所有方块逆时针旋转3*90=270度
```
=======
# 岛三速建

## 文档说明

本文档中的代码，如果出现“-snip-”表示省略了上文中重复的代码

## 建筑代码

### 岛三的建筑代码

voxels.setVoxel()可以指定最多5个参数：X, Y, Z, voxel, rotation

#### 限制

参数X, Y, Z必须是string；voxel, rotation可以是string或者number类型

```javascript
voxels.setVoxel(X, Y, Z, voxel, rotation)
/*
(x: number, y: number, Z: number, voxel: string | number, rotation?: string | number) : number
*/
```

### 举例

如 `voxels.setVoxel(1, 1, 1, 'grass', 0)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为0即方块旋转0*90=0度

如 `voxels.setVoxel(1, 1, 1, 'grass', 1)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为1即将方块逆时针旋转1*90=90度

又如 `voxels.setVoxel(1, 2, 3, 'stone', 2)`，可以在x=1,y=2,z=3的位置放置一个石头，因为旋转（rotation）的值为2，所以会将原始的方块逆时针旋转2*90=180度

`voxels.setVoxel(12, 3, 45, 'glass', 3)`，在x=12,y=3,z=45的位置放置一个玻璃方块，逆时针旋转3*90=270度

`voxels.setVoxel(12, 3, 45, 'dirt', 4)`，在x=12,y=3,z=45的位置放置一个土方块，逆时针旋转了4*90=360度，所以相当于不旋转，作用效果等于 `voxels.setVoxel(12, 3, 45, 'dirt', 0)`

说明：rotation值可以不加，默认为0

### 返回值

#### 方块存在时

如果传入的方块存在，使用此方法的返回值会返回第四个参数即voxel对应的方块ID

例如 `voxels.setVoxel(1, 2, 3, 'stone')`会返回名为“stone”的方块对应的id

#### 方块不存在时

如果方块不存在，会返回0

例如 `voxels.setVoxel(1, 2, 3, 'this_is_not_a_block_name')`会返回0

## 快速建造

快速建造可以更高效地批量化建筑方块

### 建造一个长方体

```javascript
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}
```

#### 举例

```javascript
// 定义函数
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}

// 调用函数
// 调用快速建造函数用“grass”（草方块）建造一个起于{x=1,y=1,z=1}，止于{x=100,y=64,z=101}，所有方块都旋转3*90=270度的长方体
quick_build('grass', 1, 1, 1, 100, 64, 101, 3)
// 调用快速建造函数用“stone”（草方块）建造一个起于{x=2,y=3,z=4}，止于{x=100,y=64,z=101}，此时不传入参数rotation，方块默认不旋转
quick_build('stone', 2, 3, 4, 100, 64, 101, 3)
```

#### 解决分不清x,y,z的最大值和最小值的问题

有时候并不知道xmin,ymin,zmin,xmax,ymax,zmax到底该传入什么值，以下两种方法可以解决：

##### 如果已经知道定值，可以自行判断

例如：

```javascript
var pos1 = new GameVector3(1,1,1)
var pos2 = new GameVector3(5,5,5)
```

因为pos1的x、y、z值都小于pos2的x、y、z值，所以此时应如此传入：

```javascript
quick_build('方块名', pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos3.z)
```

##### 如果两坐标完全随机，可以使用函数判断

```javascript
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	-snip-
}
function quick_build_pro(voxel, pos1, pos2, rotation=0){
	// 判断pos1和pos2的位置关系并正确传入
	if(pos1.x<=pos2.x&&pos1.y<=pos2.y&&pos1.z<=pos2.z){ // 当pos1的xyz坐标均小于等于pos2的xyz坐标时的调用方式
		quick_build(voxel, pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos2.z, rotation)
	}
	else if(pos1.x>pos2.x&&pos1.y>pos2.y&&pos1.z>pos2.z){ // 当pos2的xyz坐标均小于pos1的xyz坐标时的调用方式
		quick_build(voxel, pos2.x, pos2.y, pos2.z, pos1.x, pos1.y, pos1.z, rotation)
	}
	else{ // 否则输出错误
		console.error('不支持的判断类型')
	}
}
```

### 以某一位置为中心建造球体

```javascript
/**
 * 快速建造一个球体
 * 
 * @param {GameVector3} centerPos - 球体中心位置
 * @param {number | string} voxel - 方块id或名称
 * @param {number} r - 球体半径
 * @param {number | string} rotation - 方块旋转
*/
function ball(centerPos, r, voxel, rotation=0){
	// 创建嵌套循环，这样创建的妙处在于不必遍历地图每个方块，如果遍历地图每个方块的话地图会崩溃
	for(let x=centerPos.x-r;x<=centerPos.x+r;x++){
		for(let y=centerPos.y-r;y<=centerPos.y+r;y++){
		for(let z=centerPos.z-r;z<=centerPos.z+r;z++){
        	const position2 = new GameVector3(x, y, z);

                // 计算两个位置之间的距离
                const distance1 = Math.sqrt(Math.pow(position2.x - centerPos.x, 2) + Math.pow(position2.y - centerPos.y, 2) + Math.pow(position2.z - centerPos.z, 2));
          	if(distance1<=r){// 如果距离小于传入的r的值，则放置方块
                     	voxels.setVoxel(x,y,z,voxel,rotation)
            	}
                }
            	}
     	}
}
```

#### 限制

因为神奇代码岛的服务器能力问题，当r过大时可能会导致服务器崩溃，所以不要传入一个较大的值

#### 举例

```javascript
function ball(centerPos, r, voxel, rotation=0){
	-snip-
}

var center = new GameVector3(50, 50, 50)
ball(center, 10, 'dirt', 2) // 以{x=50,y=50,z=50}为球体中心、填充旋转了2*90=180度的“dirt”（草方块），半径为10，快速建造一个球体
```

### 在某一位置创建底面为l，高为l的三棱锥

```javascript
function pyramid(l, pos, voxel, rotation){
	let cx = pos.x;
	let cy = pos.y;
	let cz = pos.z;
	let height = l;
	let xend = cx + l;
	let zend = cz + l;
	for(let y = cy; y < cy + height; y++){
	  	let ylevel = y - cy;
	  	let xstart = cx + ylevel;
	  	let xend = cx + l - ylevel;
	  	let zstart = cz + ylevel;
	  	let zend = cz + l - ylevel;
	  	for(let x = xstart; x < xend; x++){
	    	for(let z = zstart; z < zend; z++){
	      		voxels.setVoxel(x, y, z, voxel, rotation);
	    	}
	  	}
	}
}
```

#### 举例

```javascript
function pyramid(l, pos, voxel, rotation){
	-snip-
}
var pos = new GameVector3(60,10,60)
pyramid(5, pos, 'stone', 3); // 在{x:60,y:10,z:60}使用“stone”（石头）建造一个底面为5*5，高度为5的三棱锥，所有方块逆时针旋转3*90=270度
```
>>>>>>> ca2e10112861de51453ebd6c23254832e6713bbd
>>>>>>> 9d407ff9fa37673dc2906501a380cf67ec57f121
