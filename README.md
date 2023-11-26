Previously, performing optical character recognition (OCR) in machine learning was a difficult task. There were a few libraries and models available, but they were not unified, which meant that users had to resort to third-party paid solutions.


The nougat-op library changes this by leveraging the Nougat Deep Learning Model from Meta to perform OCR on any academic PDFs and extract the text.


**To use the library, you will need Python 3.8 or higher.**

#### How to install?
```
pip install nougatop
```

Here are some reasons why you should use the nougat-op library:


* It can extract text from any type of academic PDF.
* It is more powerful than conventional methods like PDF parsers.
* It provides 100% accurate outputs.
* You can choose to extract the text with or without the LaTeX formatting.
* It can handle large PDF files.
* It is open source.

#### Example

**For converting pdf to text**
```Python
from nougatop import pdf_totext
# pdf_totext([file_path], [output_directory])
pdf_totext("/content/2006.05873.pdf","/content/ai" )
```
**For displaying the extracted text**
```Python
from nougatop import display_totext
# displaying the output (stored in .mmd file) with and without removing latex formatting
display_totext([file_path], [remove_special=False]) # by default remove_special, set to False. Meaning Latex will be added. If set True, latex formatting will be removed.
``` 

**Upcoming updates include the ability to process batch PDFs.**


**The project is licensed under MIT, and anyone is free to contribute. Please raise an issue before committing.**

