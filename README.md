# TextRecognition
This project is to achieve text recognition of 80% and above accuracy on the handwritten characters in the image and output the detected characters using different OCR tools. In order to recognize the handwritten characters more efficiently, image preprocessing must be done before the text detection process. The quality of the image is crucial as it will affect the accuracy of the text detection by OCR tools as the lower the quality of the image, the lower the chance of a character can be detected. Hence, a variety of image preprocessing techniques is performed to improve the quality of the image. For example, Pytesseract, EasyOCR, and KerasOCR are used.
# Train dataset
The Tesseract has three sets of the main dataset, which are tessdata, tessdata_fast and tessdata_best. These datasets consist of over 100 languages and 35 scripts. To name a few of the languages, it includes English (eng), Malay (msa), Chinese - Simplified (chi_sim), Chinese - Traditional (chi_tra), Tamil (tam) etc. For this project, the tessdata dataset is used to avoid any incompatibility with Tesseract’s version, as it has both the legacy models (--oem 0) and newer LSTM models (--oem 1). In terms of accuracy and speed, the tessdata is faster than tessdata-best but slightly less accurate than tessdata-best. Besides, it is also not retrainable. The tessdata LSTM models (-- oem 1) have recently been updated to the integerized versions of tessdata_best on GitHub. So, they should be faster but probably still a little less accurate than tessdata_best.
# Test dataset
## test_v2
The test_v2 is a public domain dataset that was obtained from Kaggle. It consists of more than four hundred thousand handwritten names collected through charity projects. Text recognition utilizes image processing technologies to convert characters on scanned documents into digital forms. It typically performs well in machine-printed fonts. However, it still poses difficult challenges for machines to recognize handwritten characters because of the enormous variation in individual writing styles. The inspiration of this is to explore the task of classifying handwritten text and to convert handwritten text into the digital format using various approaches out there
# System Flowchart
![image](https://user-images.githubusercontent.com/70791269/136901805-3f276063-c15e-4652-a2a5-8261837b7610.png)

For more information, see https://github.com/tesseract-ocr/tesseract and https://tesseract-ocr.github.io/tessdoc
