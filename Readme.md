# gtest2html

This project consists of a simple Python3 script to transform a [googletest][1] xml-report to responsive HTML5 using [Twitter Bootstrap 4][2] including [jQuery][3] and the jQuery Plugin [Stacktable.js][4].

## Usage

Run your googletest executable using the following commandline parameters:

```bash
./gtest-executable --gtest_output=xml:report-file.xml
```

Call gtest2html by specifying the input xml report and the path to the output directory including the name of the target HTML-file.

```bash
python3 gtest2html.py report-file.xml output/index.html
```

The complete HTML-stuff is copied inside the target directory `output`. Open `output/index.html` to view your googletest report as HTML.

## Running the example

A example googletest report is located under `example/report.xml`. To generate a respective HTML-page using gtest2html run the following commands:
```
git clone https://gitlab.uni-koblenz.de/astahlhofen/gtest2html.git

cd gtest2html

python3 gtest2html.py example/report.xml output/index.html
```

Finally open the file `output/index.html` in your favorite browser.

