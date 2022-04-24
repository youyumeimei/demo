# Progress Report for CS304

## Group Introduction

Group name: *Lanrand*  

Group members: 

- 11910213 薛丁元(XUE Dingyuan)
- 11910338 刘思岑(LIU Sicen)
- 11912627 孟宇阳(MENG Yuyang)
- 11912732 马子晗(MA Zihan)
- 11912733 黄颖盈(HUANG Yingying)

------

(a) issues chosen and reason

| issues            | reason                                                       |
| ----------------- | ------------------------------------------------------------ |
|                   |                                                              |
| 130               | 自从iphone的诞生，并且其在中国市场快速流行起来，而IOS系统有一种类型的照片格式，其格式就是HEIC格式。因此在较大的一部分中国受众中，都存在着HEIC格式的照片，所以能够将这种照片格式直接转成PDF是非常重要的。因此我选择尝试修复这个bug，以满足iOS使用者的便利。 |
|                   |                                                              |
| OpenPDF issue#620 | This issue is important for the function to set keepTogether, it no one fix it, the leading cannot be set when you want to make a paragraph keep together. This bug is caused by a commit for another issue, so it's very important to perfect it so that the fixed function can be used. This bug can be found when you write a pdf file, and may be hard to find when you just see the code, so it's important to fix it in time so that it won't affect the user experience. |
|                   |                                                              |

(b) test scenario

| issues            | test scenario                                                |
| ----------------- | ------------------------------------------------------------ |
|                   |                                                              |
|                   |                                                              |
|                   | 在修复bug之前，当运行HEIC图片转PDF的时候，会报错而无法导出成功HEIC的image。但是在修改这个错误之后，我开始测试HEIC图片转PDF是否能够成功。第一个测试只是单独测试图片是否能够转成功，运行结束之后，可以看到导出的pdf中，成功转成了PDF的HEIC图片。第二个测我将多种图片同时运行导出PDF，可以发现也成功导出了。这正是我们想要的。 |
| OpenPDF issue#620 | Before fixing the bug, when running the fuction of writing a pdf file, and set the paragraph is together, you can see that whatever leading you set, it will show the same leading. But after fixing the bug, when you set together of a paragraph, you can see the leading is what you set. And we test two cases. One is for short paragraph as the one who bring out this issue, it can be seen that the leading can be set the same as when you not use setTogether and it's what we want. We also test a long paragraph, and we can see that in the pdf file, the leading of the paragraph is what we want. |
|                   | 在修复bug之前，当运行编写pdf文件的功能时，将段落设置在一起，可以看到无论设置了什么前导，它都会显示相同的前导。但是在修正了这个错误之后，当你设置一个段落的时候，你可以看到你设置的前导。我们测试了两种情况。一个是作为引出这个问题的短段落，可以看到，前导可以设置为和不使用setTogether时一样，这就是我们想要的。我们还测试一个很长的段落，我们可以看到在pdf文件中，段落的开头是我们想要的。 |



(c) user story

| issues            | user story                                                   |
| ----------------- | ------------------------------------------------------------ |
|                   |                                                              |
|                   |                                                              |
|                   | 重新编写了一个getHeicImage方法，需要解决HEIC不支持导出的问题。用于转变HEIC图片格式为PNG图片格式，并导入出到PDF中。PR: https://github.com/LibrePDF/OpenPDF/pull/716 |
| OpenPDF issue#620 | The leading cannot be set when write a pdf file with using the function of setTogether, so it need to be fixed of the problem of setting the leading.   pr: https://github.com/LibrePDF/OpenPDF/pull/715 |
|                   | 使用setTogether函数写pdf文件时不能设置前导，需要解决前导设置的问题。公关:https://github.com/LibrePDF/OpenPDF/pull/715 |

(d) run Checkstyle, SpotBugs, and PMD

All run well.

(e) Javadoc comments

See the file of code.

(f) JUnit tests

See the file of code.

(g) schedule

| week | schedule                                         |
| ---- | ------------------------------------------------ |
| 12   | Checking the issue and look for the bugs         |
| 13   | Fixing the bugs and features                     |
| 14   | Checking the code and write Javadoc and comments |
| 15   | Finish fixing the issues and commit the PR.      |

(h) 

select TA: D

time slot: 5