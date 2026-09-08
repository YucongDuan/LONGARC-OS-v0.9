[English project overview](README.md)

# LONGARC OS v0.9 完整交付包

Created by Yucong Duan (段玉聪).

LONGARC OS（长弧）是一个面向极长时程科研任务的开源候选系统。它不依赖让同一个 Agent 永久运行，而是通过使命宪章、预登记合同、分离的生成与评估、哈希账本、检查点、可复现胶囊、未知残余、有限行动许可和继承包，让研究在模型、团队、机构与机器人更换后仍可审计地继续。

## 本包内容

- `longarc_os_v0_9_source.zip`：GitHub-ready 源码、Schema、测试、参考运行与开源治理文件。
- `longarc_os_standalone_demo.html`：无需安装、可直接在浏览器打开的离线驾驶舱。
- `longarc_os_extreme_horizon_system_report.docx`：可编辑技术报告。
- `longarc_os_extreme_horizon_system_report.pdf`：固定版式技术报告。
- `ui_previews/`：六个主要界面的视觉预览与总览图。
- `validation_summary.json`：测试、参考指标、文档质检和证据边界。
- `SHA256SUMS.txt`：本交付包中所有文件的完整性校验值。

## 快速运行

解压源码包，进入 `longarc_os_v0_9`：

```bash
python run.py demo --epochs 12 --out outputs/demo
python run.py verify --root outputs/demo
python run.py serve --root outputs/demo --port 8768
python -m unittest discover -s tests -v
```

浏览器打开：`http://127.0.0.1:8768/dashboard.html`

## 证据边界

当前版本属于作者侧确定性参考实现。它证明软件机制能够运行、恢复、保留失败、生成继承包并阻止物理动作；它不证明已经实现多年现实自治、不受约束的 AI 发明、自然科学新定律发现或安全的真实机器人控制。进入真实实验室或机器人前，必须进行独立复现、受控数据接入、硬件在环、安全控制、人工授权与领域认证。

## GitHub 状态

源码已经按 Apache-2.0、CITATION、CONTRIBUTING、GOVERNANCE、SECURITY、NOTICE、SBOM、GitHub Actions 和完整性清单组织，可直接用于建立公开仓库。当前交付未由本助手实际上传到段玉聪 GitHub，仓库名称、维护者、共同贡献者、安全联系人和最终公开声明仍需本人确认。
