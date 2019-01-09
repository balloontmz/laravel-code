## laravel shop
1. 下载源码
2. 安装依赖  composer install 、yarn install
3. .env 文件配置
4. 导入 admin.sql 文件
5. npm run dev 运行前端文件进行测试

--------------------------------------------------------------
error: The Mix manifest does not exist
解决方法：npm run dev
--------------------------------------------------------------
note：
一个小问题，生成订单的 Service 中，有一个队列任务，关于超时关闭订单的任务。此任务应该延时执行，
否则将出现产生订单立即关闭订单的情况。或者，可以干脆在此处关闭该功能