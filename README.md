# 北京大学相关 GitHub 仓库收集

本仓库收集、整理与 [北京大学](https://www.pku.edu.cn/)（PKU / 北大）相关的
GitHub 仓库，重点覆盖教务系统辅助工具、校内平台项目、课程资料与通用资源。

> 数据以 GitHub API 采集和规则初筛为起点，最终收录以人工复核为准。

## 当前收录

<!-- stats:start -->
| 分类 | 仓库数 |
| --- | ---: |
| 教务系统相关 | 60 |
| 校内其他平台相关 | 47 |
| 课程相关资料 | 320 |
| 通用资源与工具 | 40 |
| **合计** | **467** |

候选仓库 2098 个；另有 0 个可能相关的仓库等待人工复核。

信息最后更新：2026-09-18。
<!-- stats:end -->

## 仓库结构

| 目录 | 内容 |
| --- | --- |
| [教务系统相关/](./教务系统相关/) | 选课、成绩、课表、评教、门户等教务辅助工具 |
| [校内其他平台相关/](./校内其他平台相关/) | 校园网、图书馆、校园卡、树洞与校园应用等项目 |
| [课程相关资料/](./课程相关资料/) | 各门课程的讲义、作业、实验、笔记与往年题 |
| [通用资源与工具/](./通用资源与工具/) | 模板、经验、导航、升学与校园生活资源 |
| [data/](./data/) | 结构化的候选、收录与待复核数据 |
| [scripts/](./scripts/) | GitHub 搜索、初筛和 Markdown 生成脚本 |

以上数量、各分类文档和更新时间由 `scripts/build.py` 自动生成。初次使用请运行：

```powershell
python scripts/collect.py
python scripts/enrich.py
python scripts/build.py
```

可设置 `GITHUB_TOKEN` 提高 API 配额；不设置时脚本也可使用 GitHub 的匿名配额，
并会复用 `data/cache/` 中的响应。

## 收录原则

- 仓库内容须与北京大学的课程、校园系统、校园生活或通用资源有直接关系。
- 课程资料须由仓库说明、课程文件、校内链接、PKU topic 或作者公开身份等证据交叉确认；
  只有作者名含 PKU、通用作业内容或无法佐证的仓库名称时不收录。
- 仅在作者简介、论文署名或致谢中出现“北京大学 / PKU”的通用科研项目不收录。
- Fork、镜像和内容重复的仓库一般只保留信息更完整或仍在维护的版本。
- 可能相关但证据不足的项目进入 `data/review.json`，不会直接出现在分类目录中。
- 仓库可能已经失效，使用第三方工具时请自行审查代码，勿向不可信项目提交账号密码。

## 数据字段

结构化数据保留仓库名、URL、描述、创建时间、最后推送时间、主要语言、topics、
分类、命中依据与复核状态。分类文档按最后推送时间倒序排列。

## 相关聚合项目

- [ha0xin/awesome-PKU](https://github.com/ha0xin/awesome-PKU)：与本项目最接近，汇总北大工具、课程资料与论文模板。
- [PkuLilBoat/awesome-pku](https://github.com/PkuLilBoat/awesome-pku)：北大 GitHub 生态、课程与校园工具导航。
- [lib-pku/libpku](https://github.com/lib-pku/libpku)：规模较大的北京大学课程资料民间整理。
- [StephenQSstarThomas/CourseCommunity](https://github.com/StephenQSstarThomas/CourseCommunity)：多学科课程笔记互助分享平台。
- [pku-typst/awesome-PKU-Typst](https://github.com/pku-typst/awesome-PKU-Typst)：北京大学 Typst 资源专题合集。

## 致谢

目录设计与数据整理思路参考了
[Littlefish12138/UCAS-on-Github](https://github.com/Littlefish12138/UCAS-on-Github)。
