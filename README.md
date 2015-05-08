# puzzle
<p>a puzzle game 拼图游戏</p>
<p>简单的是手指点点，华容道那种，puzzle.html</p>
<p>另一个比较复杂的，是散开来再拼到一起去的，纯DOM做性能不好，没有上线。pintu.html</p>
<pre>
puzzle.init({
		width:300	//拼图宽度 默认取父元素宽度	
		,col:3	//拼图每行的格子数 默认5
		,row:4	//行数 默认5
		,hard:15	//难度系数 默认5
		,img:"example.jpg"//拼图图片路径 默认"8.jpg" 图片路径找不到时会报错
		,bgcolor:'#eee' //拼版背景颜色，格子之间缝隙的颜色 默认白色'#fff'
		,bgimg:null 	//拼版背景图片 默认空
		,type:'timeout'	//游戏模式 timeout 倒计时模式 默认timing计时模式
		,time:30	//倒计时模式下的时间限制秒数
		,success:function(time,step){alert("成功！"+time+"秒 "+step+"步")} //游戏成功执行函数 自带用时和步数参数
		,timeout:function(time,step){alert("超时！"+time+"秒 "+step+"步")} //游戏超时执行函数 自带用时和步数参数
	});

</pre>
