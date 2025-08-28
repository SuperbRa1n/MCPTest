# FastMCP Server

一个基于 FastMCP 的最小可运行 MCP Server 示例。

## 安装

建议使用虚拟环境：

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## 运行

该服务器通过 stdio 与 MCP 客户端通信。可以使用官方 Inspector 进行连接测试：

```bash
npx @modelcontextprotocol/inspector --command "python server.py"
```

或直接运行（供集成环境连接）：

```bash
python server.py
```

## 提供的工具

- `ping()`：健康检查，返回 `pong`。
- `echo(text)`：回声，返回输入文本。

## 参考

- FastMCP 文档：`https://github.com/modelcontextprotocol/fastmcp`
