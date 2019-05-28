# HTMLPDFConversion

HTMLPDFCONVERSION is a Node library for dealing with conversion of HTML content to PDF file .

## Installation

Use the package manager [npm](https://www.npmjs.com/package/htmlpdfconversion) to install htmlpdfconversion.

```bash
npm install htmlpdfconversion
```
##Sample Request
 
Var request = {
   "html": 'html content' ,
   "author" : "xyz"  //This field is optional
 }


## Usage

```npm
var htmlpdfconversion = require('htmlpdfconversion');


>htmlpdfconversion.convertPdfWithAuthorNameInHeader(request) # returns 'PDF in a Folder With Author Name in Header'

>htmlpdfconversion.convertPdf(request) # returns 'PDF in a Folder with PDF content'

Sample Function Calling
htmlpdfconversion.convertPdfWithAuthorNameInHeader(request, function(err,res){
    if (err) return console.log(err);
})
```

##NOTE
Verify JSON For multiple Line Html content. Please verify the Valid JSON.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT]