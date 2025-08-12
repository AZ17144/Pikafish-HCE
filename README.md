<div align="center"   “中心”   “中心”   “中心”   “中心”   “中心”   “中心”   “中心”   “中心”>   对齐

## About Pikafish-HCE   ## 关于 Pikafish-HCE
Pikafish-HCE is a fork of Pikafish that uses classical evaluation (handcrafted evaluation) instead of NNUE evaluation. This version has a higher NPS compared to the NNUE version, but it is weaker by about several hundred Elo. With very long time control, Pikafish-HCE has surpassed the previously strongest open-source HCE engine, NewGG.Pikafish-HCE 是 Pikafish 的一个分支版本，它采用的是传统评估（手工评估）而非 NNUE 评估。与 NNUE 版本相比，此版本的每秒计算步数（NPS）更高，但棋力弱约几百个等级分。在时间控制非常长的情况下，Pikafish-HCE 已经超越了此前最强的开源 HCE 引擎 NewGG。

  [![Pikafish][pikafish-logo]][website-link]


  <h3>Pikafish</h3>

  A free and strong UCI xiangqi engine.一款免费且强大的国际象棋引擎。
  <br>
  <strong>[Explore Pikafish docs »][wiki-link]</strong>【探索 Pikafish 文档 »】[维基链接]
  <br>
  <br>
  [Report bug][issue-link]   [报告错误][问题链接]
  ·
  [Open a discussion][discussions-link][开启讨论][讨论链接]
  ·
  [Discord   不和][discord-link]
  ·
  [Blog   博客][website-blog-link]

  [![Build   构建][build-badge]][build-link]
  [![License   许可证][license-badge]][license-link]
  [![RuleBook][rulebook-badge]][rulebook-link]
  <br>
  [![Release][release-badge]][release-link][![发布][发布徽章][发布链接]
  [![Commits][commits-badge]][commits-link][![提交记录][提交记录徽章][提交记录链接]
  <br>
  [![Website][website-badge]][website-link][![网站][website-badge]] [website-link   网站链接]
  [![Fishtest][fishtest-badge]][fishtest-link]
  [![Discord][discord-badge]][discord-link]

 
</div>

## Overview   # #概述

[Pikafish][website-link] is a **free and strong UCI xiangqi engine** derived from[Pikafish][网站链接] 是一款源自于……的免费且强大的 UCI 象棋引擎。
[Stockfish][stockfish-link] that analyzes xiangqi positions and computes the optimal moves.[Stockfish   鳕鱼干][stockfish-link] 这款程序能够分析象棋局势并计算出最佳走法。

Pikafish **does not include a graphical user interface** (GUI) that is requiredPikafish **不包含所需的图形用户界面**（GUI）
to display a chessboard and to make it easy to input moves. These GUIs are用于展示棋盘并方便输入走法。这些图形用户界面是
developed independently from Pikafish and are available online. **Read the独立于 Pikafish 开发而成，可在线获取。**阅读详情
documentation for your GUI** of choice for information about how to use有关如何使用您所选图形用户界面（GUI）的文档信息
Pikafish with it.   用它来对付棘鱼。

See also the Pikafish [documentation][wiki-usage-link] for further usage help.另请参阅 Pikafish 的[文档][wiki-usage-link]以获取更多使用帮助。

## Files   # #文件

This distribution of Pikafish consists of the following files:此 Pikafish 发行版包含以下文件：

  * [README.md][readme-link], the file you are currently reading.* [README.md][readme-link]，即您当前正在阅读的文件。

  * [Copying.txt][license-link], a text file containing the GNU General Public* [Copying.txt][许可链接]，一个包含 GNU 通用公共许可证的文本文件
    License version 3.   License版本3。

  * [AUTHORS][authors-link], a text file with the list of authors for the official Pikafish project.

  * [src][src-link], a subdirectory containing the full source code, including a* [源代码][源代码链接]，一个包含完整源代码的子目录，其中包括一个
    Makefile that can be used to compile Pikafish on Unix-like systems.可在类 Unix 系统上用于编译 Pikafish 的 Makefile 文件。

  * a file with the .nnue extension, storing the neural network for the NNUE一个带有.nnue 扩展名的文件，用于存储 NNUE 的神经网络。
    evaluation.   评估。

## Contributing   # #贡献

__See [Contributing Guide](./CONTRIBUTING.md).__请参阅[贡献指南](./CONTRIBUTING.md)。

### Donating hardware

Improving Pikafish requires a massive amount of testing. You can donate your
hardware resources by installing the [Fishtest Worker][worker-link] and viewing
the current tests on [Fishtest][fishtest-link].

### Improving the code

In the [chessprogramming wiki][programming-link], many techniques used in
Pikafish are explained with a lot of background information.
The [section on Stockfish][programmingsf-link] describes many features
and techniques used by Stockfish. However, it is generic rather than
focused on Stockfish's precise implementation.

The engine testing is done on [Fishtest][fishtest-link].
If you want to help improve Pikafish, please read this [guideline][guideline-link]
first, where the basics of Pikafish development are explained.

Discussions about Pikafish take place these days mainly in the Pikafish如今有关皮卡鱼的讨论主要在皮卡鱼社区进行。
[Discord server][discord-link]. This is also the best place to ask questions
about the codebase and how to improve it.关于代码库以及如何改进它。


## Compiling Pikafish   编译Pikafish

Pikafish has support for 32 or 64-bit CPUs, certain hardware instructions,
big-endian machines such as Power PC, and other platforms.

On Unix-like systems, it should be easy to compile Pikafish directly from the
source code with the included Makefile in the folder `src`. In general, it is
recommended to run `make help   使帮助` to see a list of make targets with corresponding
descriptions.   描述。

```
cd src
make -j build ARCH=x86-64-modern使用命令 `make -j build ARCH=x86-64-modern` 进行构建。
```

Detailed compilation instructions for all platforms can be found in our
[documentation   文档][wiki-compile-link]   (wiki-compile-link)   (wiki-compile-link). Our wiki also has information about
the [UCI commands][wiki-uci-link] supported by Pikafish.

## Terms of use   ##使用条款

### GNU General Public License version 3

Pikafish is free and distributed under the
[**GNU General Public License version 3GNU 通用公共许可证第 3 版**][license-link] (GPL v3). Essentially,
this means you are free to do almost exactly what you want with the program,
including distributing it among your friends, making it available for download
from your website, selling it (either by itself or as part of some bigger
software package), or using it as the starting point for a software project of
your own.

The only real limitation is that whenever you distribute Pikafish in some way,
you MUST always include the license and the full source code (or a pointer to
where the source code can be found) to generate the exact binary you are
distributing. If you make any changes to the source code, these changes must
also be made available under GPL v3.

[authors-link]:			https://github.com/official-pikafish/Pikafish/blob/master/AUTHORS
[build-badge]:			https://img.shields.io/github/actions/workflow/status/official-pikafish/Pikafish/pikafish.yml?branch=master&style=for-the-badge&label=pikafish&logo=github
[build-link]:				https://github.com/official-pikafish/Pikafish/actions/workflows/pikafish.yml
[commits-badge]:		https://img.shields.io/github/commits-since/official-pikafish/Pikafish/latest?style=for-the-badge
[commits-link]:			https://github.com/official-pikafish/Pikafish/commits/master
[discord-badge]:			https://img.shields.io/discord/1013130558089478144?style=for-the-badge&label=discord&logo=Discord
[discord-link]:			https://discord.com/invite/uSb3RXb7cY
[discussions-link]:   https://github.com/official-pikafish/Pikafish/discussions/new
[fishtest-badge]:			https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=Fishtest&up_color=success&up_message=Online&url=https://test.pikafish.org
[fishtest-link]:			https://test.pikafish.org
[guideline-link]:			https://github.com/glinscott/fishtest/wiki/Creating-my-first-test
[issue-link]:         https://github.com/official-pikafish/Pikafish/issues/new?assignees=&labels=&template=BUG-REPORT.yml
[license-badge]:			https://img.shields.io/github/license/official-pikafish/Pikafish?style=for-the-badge&label=license&color=success
[license-link]:			https://github.com/official-pikafish/Pikafish/blob/master/Copying.txt
[pikafish-logo]:			https://pikafish.org/assets/logo_256.png
[programming-link]:		https://www.chessprogramming.org/Main_Page
[programmingsf-link]:	https://www.chessprogramming.org/Stockfish
[qqgroup-link]可在类 Unix 系统上用于编译 Pikafish 的 Makefile 文件。:			https://jq.qq.com/?_wv=1027&k=FORWUh4W
[readme-link]:			https://github.com/official-pikafish/Pikafish/blob/master/README.md
[release-badge]可在类 Unix 系统上用于编译 Pikafish 的 Makefile 文件。:			https://img.shields.io/github/v/release/official-pikafish/Pikafish?style=for-the-badge&label=official%20release
[release-link]:			https://github.com/official-pikafish/Pikafish/releases/latest
[rulebook-badge]:		https://img.shields.io/badge/computer%20rule-20B2AA?style=for-the-badge&logo=mdbook
[rulebook-link]:			https://pikafish.org/rule.pdf
[src-link]:				https://github.com/official-pikafish/Pikafish/tree/master/src
[stockfish-link]:			https://github.com/official-stockfish/Stockfish
[uci-link]:				https://backscattering.de/chess/uci/
[website-badge]:		https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=website&up_color=success&up_message=Online&url=https://pikafish.org
[website-link]:			https://pikafish.org
[website-blog-link]:  https://pikafish.org/
[wiki-link]:          https://github.com/official-pikafish/Pikafish/wiki
[wiki-compile-link]:  https://github.com/official-pikafish/Pikafish/wiki/Compiling-from-source
[wiki-uci-link]:      https://github.com/official-pikafish/Pikafish/wiki/UCI-&-Commands
[wiki-usage-link]:    https://github.com/official-pikafish/Pikafish/wiki/Download-and-usage
[worker-link]:			https://github.com/xyztnecniV/yolo
