
 <h1 class="curproject-name"> GitMonitor </h1> 
 检测github，gitee开源仓库是否存在敏感信息


# 身份认证类

## 扫描github仓库
<a id=扫描github仓库> </a>
### 基本信息

**Path：** /asa_gitmonitor/api/search/github

**Method：** POST

**接口描述：**
<p>in_name 如果不填默认读取user下所有仓库</p>


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/json | 是  |   |   |
| X-GIT-TOKEN  |  123... | 是  |   |  身份验证token |
**Body**

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> user</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3>mengjiaheng</td><td key=4><span style="white-space: pre-wrap">github用户名</span></td><td key=5><p key=5><span style="font-weight: '700'">mock: </span><span>mengjiaheng</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> in_name</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">仓库名</span></td><td key=5></td></tr>
               </tbody>
              </table>
            
### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3>200</td><td key=4><span style="white-space: pre-wrap">请求状态码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> message</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3>success</td><td key=4><span style="white-space: pre-wrap">请求信息</span></td><td key=5></td></tr>
               </tbody>
              </table>
            
