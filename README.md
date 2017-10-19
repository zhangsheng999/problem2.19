# problem2.19\
### 题目大意
模拟一个在空中旋转飞行的棒球，且假定自转角速度2000rpm.
### 解答
棒球的运动方程
m*d²r/dt²=F

F=m*g+B/m*v²*v/|v|+S*v×w

Fmagnus=Sv×w

Xi+1=Vx,i*∆t+Xi

Yi+1=Vy,i*∆t+Yi

Zi+1=Vz,i*∆t+Zi

Vx,i+1=Fx*∆t+Vx,i

Vy,i+1=Fy*∆t+Vy,i

Vz,i+1=Fz*∆t+Vz,i

由上述公式可知，只要知道了前一步棒球的状态，那么棒球的下一个状态就可以由上述欧拉法的计算公式得到。 
计算得到棒球的平面内飞行轨迹如图所示
![](https://raw.githubusercontent.com/supermanvista/Computional_Physics_2013301020094/master/Photos/baseball.png)

### 情况一
 #### the ball without airdrag or spin
 
 ![](https://github.com/zhangsheng999/1111/blob/master/a.png?raw=true)
 
 [代码](https://github.com/zhangsheng999/1111/blob/master/without%20airdrag%20or%20spin.txt)
 
 
 ### 情况二
  #### the ball with airdrag
  
  ![](https://github.com/zhangsheng999/1111/blob/master/b.png?raw=true)
  
  [代码](https://github.com/zhangsheng999/1111/blob/master/with%20air%20drag.txt)
  
  ### 情况三
   #### the ball with airdrag and spin
   
   ![](https://github.com/zhangsheng999/1111/blob/master/abc.png?raw=true)
   
   [代码](https://github.com/zhangsheng999/1111/blob/master/with%20air%20drag%20and%20spin.txt)
   
   
   ##### 由上图的轨迹可以清晰地看出：在考虑棒球受到的Magnus力作用下，棒球会产生一个“回旋”运动，类似于“香蕉球”。 
### 由此可知棒球运动中，棒球的旋转运动会对棒球的轨迹产生巨大影响。
