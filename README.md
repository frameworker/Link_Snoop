# Link_Snoop
PDFKit sample

Link Snoop is a simple application using the Quartz framework, PDFKit, in Mac OS X Tiger. When a user opens a PDF with this application it scans it for Link annotations that have a URL associated with them. URL link annotations are displayed in an NSTableView. Also, the PDF is displayed with these annotations highlighted.

- It shows simple use of PDFKit including creating a PDFDocument and associating it with a PDFView.
- It shows how to subclass PDFView and override the drawing method in order to render a box around Link annotations.
- It demonstrates bounds-testing of text on a PDFPage (using PDFSelection's).
= It also demonstrates simple creaton of PDFDestination's.

Revision History

2005-06-01 Version 1.0	
Shows how to use PDFKit to scan for and highlight link annotations in PDFs.

2018-07-25 Version 2.0
Brought up-to-date in macOS 10.13.5 with Xcode 9.2
Base SDK 10.13
macOS Deployment Target 10.13
Repaired warnings and updated Deprecated APIs
Updated API usage for new PDFKit
Fixed bug that kept tableView from working
Added Read Me with Revision History and Eratta

Eratta

"Overridden deprecated methods" warning needs to be turned on and warnings repaired.

Turn on other warnings and fix issues that crop up.
https://github.com/boredzo/Warnings-xcconfig/wiki/Warnings-Explained

Wrapped-links that show on two lines are treated as two occurrances of the same link even though there should only really be one link.
