
API Automation

Installation

1. This tool requires Node to be installed! :- https://nodejs.org/en/download/
2. Editor :- https://code.visualstudio.com/download

Post Installation

1. Take pull from the repository from Automation-v2 (Sub-master branch)
2. Do an npm install

How to run file

1. Under package.json, scripts are present releaserun,qatrun,releasereports,qatreports
2. On local run npm test or npm run qatrun to run files (This will run all files having .only under it blocks)
3. npm run qatrun will run all the files on qat environment & releaserun will run on release environment


html_to_pdf.js :- This file will convert report.html to pdf & output is seen in folder PDFgeneration

slackintegration.js :- This file will push pdf report to slack channel - automation-reports

How to push report to slack

1. Run :- "npm run releasereports" command from local (This will convert html to pdf & then push the release report to slack channel :- automation-reports)
2. Now run : "npm run qatreports" command from local (This will convert html to pdf & then push the qat report to slack channel :- automation-reports)