# Job-脚本执行(GITHUB版)

# 配置
插件上架时，需要配置蓝鲸智云相关参数，路径：设置->私有配置
- BK_APP_ID:应用ID，别名bk_app_code，需要使用已添加至蓝鲸ESB接口调用白名单中的应用ID，建议使用蓝鲸开发者中心内的蓝盾调用ESB接口专用应用ID（默认为bk_ci）
- BK_APP_SECRET: 应用ID对应的安全密钥(应用TOKEN)，可以通过 蓝鲸智云开发者中心 -> 点击应用 ID -> 基本信息 获取
- ESB_HOST: 蓝鲸ESB网关地址, 若插件所运行的环境能够解析paas.service.consul，则填写http://paas.service.consul，否则填写蓝鲸平台地址，例如https://paas.bk.com
- ESB_CERTIFICATE: 若ESB_HOST为http://paas.service.consul，则无需配置该项，若ESB_HOST使用http或https证书为商业CA颁发的证书（浏览器域名左边的锁标志为关闭的锁表示连接安全），则无须配置该项，仅在ESB_HOST使用https私有证书时配置为私有证书公钥内容
- JOB_HOST: 蓝鲸JOB独立地址，比如https://job.bk.com
