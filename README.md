Introduction
------------

This module aim is to translate a string to a desired languages and save the output in a nice excel file

## Installation
Install via pip:

    pip install os-translator-xlsx

## Usage       
    
    import os_translator_xlsx.ToXlsxTranslator as excelTranslator
    
    excelTranslator.translate_to_excel('output/path/file.xlsx',
                                       '/path/to/service/account/.json',
                                       'firebaseprojectId',
                                       'en-US',
                                       ["First sentence", "Second setntence"],
                                       ['zu', 'fr'])
                                       
## Method signatures

    def translate_to_excel(excel_file_path,
                           service_account_json_path,
                           project_id,
                           language_initials_src,
                           text_list,
                           language_initials_list):
                           
        """Will translate a text to a given languages and save the results in a nice excel file.
    
        Parameters:
        :param excel_file_path: the path to the excel file with all of the translations
        :param service_account_json_path: the path to your google translate api json key. Download from your firebase's project's settings
        :param project_id: your project id (fetch from your api console project's name: https://console.cloud.google.com/?_ga=2.55756075.1423406147.1582784765-1154152733.1582784765)
        :param language_initials_src: the source language
        :param text_list: a list containing all of the texts to translate
        :param language_initials_list: the initials of the languages you want to translate to
    
        NOTICE:
            If there are substrings you don't want to translate, write KEEP before them. Example: "The boy looks KEEPWord".
            Also, you can use this bank of languages:
            ['en-GB', 'af', 'am', 'ar', 'hy-AM', 'az-AZ', 'bn-BD', 'eu-ES', 'be', 'bg', 'my-MM', 'ca', 'zh-HK', 'zh-CN', 'zh-TW', 'hr', 'cs-CZ', 'da-DK', 'nl-NL', 'en-AU', 'en-IN', 'en-SG', 'en-ZA', 'en-CA', 'en-US', 'et', 'fil', 'fi-FI', 'fr-FR', 'fr-CA', 'gl-ES', 'ka-GE', 'de-DE', 'el-GR', 'hi-IN', 'hu-HU', 'is-IS', 'id', 'it-IT', 'ja-JP', 'kn-IN', 'km-KH', 'ko-KR', 'ky-KG', 'lo-LA', 'lv', 'lt', 'mk-MK', 'ms', 'ml-IN', 'mr-IN', 'mn-MN', 'ne-NP', 'no-NO', 'fa', 'pl-PL', 'pt-BR',
                           'pt-PT', 'ro', 'ro', 'ru-RU', 'sr', 'si-LK', 'sk', 'sl', 'es-419', 'es-ES', 'es-US', 'sw', 'sv-SE', 'ta-IN', 'te-IN', 'th', 'tr-TR', 'uk', 'vi', 'zu']
        """

## Licence
MIT