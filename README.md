
---

Documentation: [English version](https://github.com/mjjonone/mjj/blob/main/README_EN.md) | 中文版

---

---

已打包成的镜像名为`mjjonone/mjj:amd64`，变量设置如下：容器的`PORT`变量可设置为3000、7860等，具体根据容器平台的要求进行设置，一般可以将`PORT`设置为3000。


---

在node.js环境中，上传`index.js`、`package.json`和`start.sh`文件，同时支持通过网址`/list`查看节点信息和`/sub`节点订阅地址。

---

Minecraft相关的服务器：
1. Vanilla Bedrock或Minecraft Bedrock，启动文件为`bedrock_server`。
2. Paper Minecraft Java，启动文件为`server.jar`。

---

1-1：在上传之前，将原来的`bedrock_server`重命名为`bedrock_server1`，然后上传`start.sh`脚本并将其重命名为`bedrock_server`。

2-1：在上传之前，将原来的`server.jar`重命名为`server1.jar`，然后上传`server.jar`和`start.sh`。

---

在`start.sh`文件中填写变量信息。

---

自动输出vless节点信息，并保存在`list.txt`文件中。

---

变量说明：

- `DEBUG`：默认为0，1代表开启，0是关闭。检测nezha的连通性
- `NEZHA_SERVER`：Nezha地址（如果没有可不填）。
- `NEZHA_PORT`：Nezha端口（如果没有可不填）。
- `NEZHA_KEY`：Nezha密匙（如果没有可不填）。
- `TLS`：默认为1，代表开启tls,如果不需要TLS，请将变量设置为0。
- `ARGO_DOMAIN`：隧道固定域名（如果没有可不填）。
- `ARGO_AUTH`：隧道的token或者json（如果没有可不填）。
- `WSPATH`：默认值为`argo`。
- `UUID`：默认值为`de04add9-5c68-8bab-950c-08cd5320df18`。
- `ARGO_AUTH`：隧道的值，请参考f佬的说明。
- 变量的填写方法也可以参考f佬的说明。

说明链接：[https://github.com/fscarmen2/Argo-X-Container-PaaS/blob/main/README.md](https://github.com/fscarmen2/Argo-X-Container-PaaS/blob/main/README.md)

