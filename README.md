Introduction
------------

This module aim is to translate a string to a desired languages and save the output in a nice excel file

## Installation
Install via pip:

    pip install os_translator_xlsx

## Usage       
    
    import os_translator_xlsx.ToXlsxTranslator as excelTranslator
    
    excelTranslator.translate_to_excel('output/path/file.xlsx',
                                       '/path/to/service/account/.json',
                                       'firebaseprojectId',
                                       'en-US',
                                       ["First sentence", "Second setntence"],
                                       ['zu', 'fr'])

## Licence
MIT