<script>
	export default {
		globalData: {
			text: 'text',
			openid: "",
			userid: "1",
		},  
		onLaunch: function() {
			//实现remove的方法
			Array.prototype.remove = function(val) {
				var index = this.indexOf(val);
				if (index > -1) {
				this.splice(index, 1);
				}
			};
		},
		onShow: function() {
			
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>
<style>
	html,page,#app {height: 100%;font-family: .PingFang SC;}
	::-webkit-scrollbar{
	
	  display: none;
	
	}
	/*每个页面公共css */
	@font-face {font-family: "iconfont";
	  src: url('https://112.74.59.218:8080/font/iconfont.eot?t=1619630357593'); /* IE9 */
	  src: url('https://112.74.59.218:8080/font/iconfont.eot?t=1619630357593#iefix') format('embedded-opentype'), /* IE6-IE8 */
	  url('data:application/x-font-woff2;charset=utf-8;base64,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') format('woff2'),
	  url('https://112.74.59.218:8080/font/iconfont.woff?t=1619630357593') format('woff'),
	  url('https://112.74.59.218:8080/font/iconfont.ttf?t=1619630357593') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+ */
	  url('https://112.74.59.218:8080/font/iconfont.svg?t=1619630357593#iconfont') format('svg'); /* iOS 4.1- */
	}
	
	.iconfont {
	  font-family: "iconfont" !important;
	  font-size: 16px;
	  font-style: normal;
	  -webkit-font-smoothing: antialiased;
	  -moz-osx-font-smoothing: grayscale;
	}
	
	.icon-pinglun:before {
	  content: "\e628";
	}
	
	.icon-send:before {
	  content: "\e6a7";
	}
	
	.icon-shoucang:before {
	  content: "\e61d";
	}
	
	.icon-liaotian:before {
	  content: "\e660";
	}
	
	.icon-dingwei:before {
	  content: "\e618";
	}
	
	.icon-fangdajing:before {
	  content: "\e637";
	}
	
	.icon-xiaoxi:before {
	  content: "\e622";
	}
	
	.icon-icon-test:before {
	  content: "\e61b";
	}
	
	.icon-fenxiang:before {
	  content: "\e654";
	}
	
	.icon-shizhong:before {
	  content: "\e72a";
	}
	
	radio .uni-radio-input{
		transform:scale(0.6);
	}
	radio.free .uni-radio-input.uni-radio-input-checked{
		background: #041746 !important;
		border-color: #041746 !important;
	}
	radio.fast .uni-radio-input.uni-radio-input-checked{
		background: #f05050 !important;
		border-color: #ff0000 !important;
	}
	radio .uni-radio-input.uni-radio-input-checked::before{
		font-size: 0rpx; /* 对勾大小 去掉 */
	}
</style>
