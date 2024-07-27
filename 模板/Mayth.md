```latex
\NeedsTeXFormat{LaTeX2e}
\ProvidesClass{Mayth}[2024/07/23 v1.0 Mayth class]
\LoadClass[oneside]{ctexbook} %小字电子版
%\LoadClass[zihao=-4]{ctexbook} %大字打印版

\RequirePackage{amsmath}
\RequirePackage{amssymb}
\RequirePackage{amsthm}
\RequirePackage{geometry}
\RequirePackage{comment}
\RequirePackage{graphicx}
\RequirePackage{pgfplots}
\RequirePackage{caption}
\RequirePackage{etoolbox}
\RequirePackage[colorlinks]{hyperref}
\RequirePackage{bookmark}
\RequirePackage{upgreek}
\RequirePackage{mathrsfs}
\RequirePackage{commath}
\RequirePackage{marginnote} %\reversemarginpar
\RequirePackage{pifont}
\RequirePackage{cite} % 引入cite包，用于处理引用
\RequirePackage{natbib} % 引入natbib包，用于处理参考文献
\RequirePackage{gbt7714} 
\RequirePackage{hyperref}


\pgfplotsset{compat=1.18}
%% 紧凑打印
%\geometry{a4paper, left=2.5cm, right=2.5cm, top=1.5cm, bottom=1.5cm}
%% 书本
\geometry{a4paper, left=4cm, right=4cm, top=3cm, bottom=3cm}
%% 16:9 PC横屏 
%\geometry{paperwidth=24cm, paperheight=13.5cm, left=1cm, right=1cm, top=1cm, bottom=1cm}
%% 4:3 ipad横屏
%\geometry{paperwidth=22cm, paperheight=16.5cm, left=1.5cm, right=1.5cm, top=1.5cm, bottom=1.5cm}

\setcounter{chapter}{-1} % 第零章开始
\setcounter{tocdepth}{1} % 目录层级为section

\theoremstyle{definition}
\newtheorem{question}{问题}[section]
\newtheorem{example}{例}[section]
\newtheorem{exercise}{练习}[section]
\newtheorem{formula}{公式}[section]
\newtheorem{definition}{定义}[section]
\newtheorem*{solution}{解}
\newtheorem{intro}{引入}[section]
\newtheorem*{property}{性质}

\theoremstyle{plain}
\newtheorem*{note}{注记}
\newtheorem*{analysis}{分析}
\newtheorem*{purpose}{设计目的}


\renewcommand{\qedsymbol}{$\blacksquare$}
\renewcommand{\proofname}{\bf 证明}
\newcommand{\pll}{\kern 0.56em/\kern -0.8em /\kern 0.56em}

\def\equationautorefname{式}
\def\footnoteautorefname{脚注}
\def\itemautorefname{项}
\def\figureautorefname{图}
\def\tableautorefname{表}
\def\partautorefname{篇}
\def\appendixautorefname{附录}
\def\chapterautorefname{章}
\def\sectionautorefname{节}
\def\paragraphautorefname{段落}
\def\subparagraphautorefname{子段落}
\def\FancyVerbLineautorefname{行}
\def\theoremautorefname{定理}
\def\exampleautorefname{例}
\def\questionautorefname{问题}
\def\exerciseautorefname{练习}
\def\formulaautorefname{公式}
\def\definitionautorefname{定义}
% 对于没有编号的环境，如 solution，通常不需要定义 \autoref 名称

\def\pgfsysdriver{pgfsys-dvipdfm.def}
\usetikzlibrary{shapes.geometric}

%定义平行且等于符号
\newcommand\pxqdy{%
    \mathrel{\text{%
            \tikz[baseline,line width=0.05ex,line cap=round]
            \draw (0,0) -- (.7em,0)
            (0,.45ex) -- (.7em,.45ex)
            (.25em,.55ex) -- (.35em,1.6ex)
            (.45em,.55ex) -- (.55em,1.6ex);}}}

%定义平行四边形符号
\newcommand\pxsbx{%
    \mathord{\text{%
            \tikz[baseline,line width=0.05ex,line join=round]
            \draw (0,.1ex) -- (.8em,.1ex) -- (1em,1.6ex) -- (.2em,1.6ex) -- cycle;}}}

% Title, author, and date
\title{\huge{\textsc{RedMath}: 我的高中数学教学笔记}}
\author{}
\date{\Large{\today}}

\endinput
```

