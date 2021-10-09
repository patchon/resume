# Stack Overflow theme for jsonresume 
This is a modified version of the [jsonresume-theme-stackoverflow](https://github.com/phoinixi/jsonresume-theme-stackoverflow), all credits goes to the creator. 

## Getting started

### Install resume-cli and build jsonresume-theme-stackoverflow-themed pdf,  
```
$ > cd ~/
$ > npm install resume-cli
$ > cd node_modules
$ > git clone git@github.com:patchon/resume.git
$ > mv resume jsonresume-theme-stackoverflow

# Set correct format and margins to fit my CV, 
$ > vim node_modules/resume-cli/build/export-resume.js (~:126)

await page.pdf({
      path: fileName + format,
      format: 'A4',
      printBackground: true,
      margin: {
        top: '20px',
        bottom: '30px',                                                                                                                                                                                                        
        right: '50px',
        left: '50px'
      },  
      ...themePkg.pdfRenderOptions
    }); 

# Create pdf, 
$ > cd ~/node_modules/jsonresume-theme-stackoverflow
$ > ~/node_modules/.bin/resume export --format pdf --theme stackoverflow mycv.pdf

```
## License

Available under the [MIT license](http://opensource.org/licenses/mit-license.php).
