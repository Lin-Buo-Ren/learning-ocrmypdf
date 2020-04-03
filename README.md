# Learning OCRmyPDF
Notes during the learning of OCRmyPDF, a Tesseract based Optical Character Recognition(OCR) software

## License
Unless otherwise specified, content in this work is release under the Creative Commons BY-SA 4.0+ license.  Most source materials are distributed under the Fair Use principle.

## References

* [OCRmyPDF documentation](https://ocrmypdf.readthedocs.io/)

## Multi-page recognition, with language presplit
```shell
$ ocrmypdf \
    --title 'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS' \
    --author '蔡英文(Ing-wen, Tsai)' \
    --language eng \
    --deskew \
    --clean \
    --skip-text \
    --pages 1,3-416 \
    --verbose 1 \
    'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS.decrypted.pdf' \
    'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS.decrypted.ocr.HanT_eng.tessdata_fast.pdf'
```

```shell
$ ocrmypdf \
    --title 'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS' \
    --author '蔡英文(Ing-wen, Tsai)' \
    --language eng \
    --deskew \
    --clean \
    --skip-text \
    --pages 2 \
    --verbose 1 \
    'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS.decrypted.pdf' \
    'UNFAIR TRADE PRACTICES AND SAFEGUARD ACTIONS.decrypted.ocr.HanT_eng.tessdata_fast.pdf'
```