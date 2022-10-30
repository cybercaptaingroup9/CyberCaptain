## SECTION 1 : PROJECT TITLE
## Intelligent carpooling system

<div align=center>
<img src="https://github.com/kaiyangHebert/CyberCaptain/blob/main/img/first%20page.jpg?raw=true" width="447" height="879"> width="180" height="105"/>
</div>


## 
  
## Install
download [Node.js](https://nodejs.org/en/download/)  
`$ npm install`  
  
download [python3.6](https://www.python.org/downloads/release/python-360/)  
`$ pip install -r requirements.txt`  

## Error and Solution  
In file:.\lib\site-packages\chatterbot\tagging.py  
**Change** `yaml.load()` **to** `yaml.safe_load() `  
  
**Change** `self.nlp = spacy.load(self.language.ISO_639_1.lower())` **to**
`if self.language.ISO_639_1.lower() == 'en': self.nlp = spacy.load('en_core_web_sm')  `
`else: self.nlp = spacy.load(self.language.ISO_639_1.lower())`

