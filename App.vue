<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	/* 官方的ui库 */
	@import "/common/uni.css";
	/* 第三放动画库 */
	@import "/common/animate.css";
	/* 自定义图标库 */
	@import "/common/icon.css";
	/* 公共样式 */
	@import "/common/common.css";
	/* 封装的样式 */
	@import "/common/zcm-main.css";
</style>
