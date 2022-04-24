# Progress Report for CS304
## Group Introduction
#### Group name: *Lanrand*

- [GitHub repository](https://github.com/orgs/cs304-2022/teams/lanrand)

#### Group members:

- 11910213 薛丁元(XUE Dingyuan)
- 11910338 刘思岑(LIU Sicen)
- 11912627 孟宇阳(MENG Yuyang)
- 11912732 马子晗(MA Zihan)
- 11912733 黄颖盈(HUANG Yingying)


### (a) Issue
| Issues | Reasons |
| --- | --- |
| [java-faker issue#386](https://github.com/DiUS/java-faker/issues/386) | BloodType is a library with less information and simple classification, which is suitable for beginning this project. Test cases are easy to construct using regular expression. |
| [java-faker issue#707](https://github.com/DiUS/java-faker/issues/707) | Java faker doesn't have methods and data to generate random and faker data  of Elden Ring. These data and methods are important because Elden Ring is one of the most popular games recently and there are people who want to use Java faker to generate data. Test cases are easy to construct using regular expression. |
| [OpenPdf issue#130](https://github.com/LibrePDF/OpenPDF/issues/130) | Since the birth of iPhone and its rapid popularity in the Chinese market, IOS system has a type of photo format, the format is HEIC format. Therefore, HEIC photos exist in a large part of the Chinese audience, so it is very important to be able to directly convert this photo format into PDF. So I chose to try to fix this bug for the convenience of iOS users. |
| [OpenPdf issue#620](https://github.com/LibrePDF/OpenPDF/issues/620) | This issue is important for the function to set keepTogether, it no one fix it, the leading cannot be set when you want to make a paragraph keep together. This bug is caused by a commit for another issue, so it's very important to perfect it so that the fixed function can be used. This bug can be found when you write a pdf file, and may be hard to find when you just see the code, so it's important to fix it in time so that it won't affect the user experience. |
| [OpenPdf issue#687](https://github.com/LibrePDF/OpenPDF/issues/687) | Openpdf is a versatile project that generates PDF files from Java code. This issue is when the project generates PDF. In some cases, pictures and words overlap, which greatly affects the use. Many users commented on this serious bug, so I tried to fix it. |


### (b) Test Scenario
| Issues | Test Scenarios | Test Scripts |
| --- | --- | --- |
| [java-faker issue#386](https://github.com/DiUS/java-faker/issues/386) | All the outputs of the methods are strings. Therefore, the first test scenario is that we assert whether the types generate by our methods match the correct regular expression we defined which should be true in Junit test. The second scenario is that we assert whether the outputs contains illegal characters which should be false in Junit test. |  |
| [java-faker issue#707](https://github.com/DiUS/java-faker/issues/707) | All the outputs of the methods are strings. Therefore, the first test scenario is that we assert whether the name, location, weapon generate by our methods match the correct regular expression we defined which should be true in Junit test. The second scenario is that we assert whether the outputs contains illegal characters which should be false in Junit test. |  |
| [OpenPdf issue#130](https://github.com/LibrePDF/OpenPDF/issues/130) | Before fixing the bug, when running HEIC image to PDF, an error will be reported and the IMAGE of HEIC cannot be exported successfully. But after correcting this error, I began to test whether HEIC pictures could be converted to PDF successfully. The first test is only a separate test to see whether the image can be successfully converted. After the operation, you can see the HEIC image successfully converted into PDF in the exported PDF. In the second test, I ran a variety of pictures at the same test and exported PDF, which was also successfully exported. This is exactly what we want. |  |
| [OpenPdf issue#620](https://github.com/LibrePDF/OpenPDF/issues/620) | Before fixing the bug, when running the fuction of writing a pdf file, and set the paragraph is together, you can see that whatever leading you set, it will show the same leading. But after fixing the bug, when you set together of a paragraph, you can see the leading is what you set. And we test two cases. One is for short paragraph as the one who bring out this issue, it can be seen that the leading can be set the same as when you not use setTogether and it's what we want. We also test a long paragraph, and we can see that in the pdf file, the leading of the paragraph is what we want. |  |
| [OpenPdf issue#687](https://github.com/LibrePDF/OpenPDF/issues/687) | This bug occurs when the user stores text and images using a Paragraph object, the first stored text and images overlap. I tested and reproduced the issue. After I fix this bug, I use Paragraph again to store the words and images, and there is no overlap. Then the second test scenario repeated the words and pictures in the Paragraph, with no overlap. |  |


### (c) Pull Request

| Issues | User Stories | Pull Request | State |
| --- | --- | --- | --- |
| [java-faker issue#386](https://github.com/DiUS/java-faker/issues/386) | The user asks for databases of blood types and ills for person forms and health systems. | [java-faker PR#134](https://github.com/datafaker-net/datafaker/pull/134) | Merged |
| [java-faker issue#707](https://github.com/DiUS/java-faker/issues/707) | Elden Ring is a hot game released recently. It is excellent and very popular, the user requests to add some features of Elden Ring in data-faker. | [java-faker PR#123](https://github.com/datafaker-net/datafaker/pull/123) | Merged |
| [OpenPdf issue#130](https://github.com/LibrePDF/OpenPDF/issues/130) | A getHeicImage method has been rewritten to address the issue that HEIC does not support exporting. Convert HEIC image format to PNG image format and import to PDF. | [OpenPdf PR#716](https://github.com/LibrePDF/OpenPDF/pull/716) | checks OK |
| [OpenPdf issue#620](https://github.com/LibrePDF/OpenPDF/issues/620) | The leading cannot be set when write a pdf file with using the function of setTogether, so it need to be fixed of the problem of setting the leading. | [OpenPdf PR#715](https://github.com/LibrePDF/OpenPDF/pull/715) | checks OK |
| [OpenPdf issue#687](https://github.com/LibrePDF/OpenPDF/issues/687) | When the user uses paragraph to generate a PDF, the text and images overlap. I fixed this bug, | [OpenPdf PR#696](https://github.com/LibrePDF/OpenPDF/pull/696) | checks OK |

### (d) Plugin



### (e) Javadoc comments

All the methods we wrote have Javadoc comments, which can be seen in our code files.

### (f) JUnit tests







### (g) schedule

| week | schedule                                         |
| ---- | ------------------------------------------------ |
| 12   | Checking the issue and look for the bugs         |
| 13   | Fixing the bugs and features                     |
| 14   | Checking the code and write Javadoc and comments |
| 15   | Finish fixing the issues and commit the PR.      |

### (h) lab session

select TA: D

time slot: 5