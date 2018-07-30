#  Main repository for docs.creolabs.com

### How it works
A script on our docs.creolabs.com server process documentation each time a new commit is pushed into this repository.
The docs folder is recursively scanned and ONLY the folders that contain a `toc.json` file are considered valid.

### toc.json
The toc.json must contain a TOC array followed by several maps items:
```
{
  "TOC": [
    {
      "entry": "INTRODUCTION"
    },
   ]
}
```

Each item can be:
* an `entry` key with a `string` value, for example:
```
{
  "TOC": [
    {
      "entry": "INTRODUCTION"
    },
    ...
   ]
}
```
this is used to group items of the same type in the left navigation section.
* a `name` and `file` entry, used to manually list a file to processed with a specified name:
```
{
  "TOC": [
    {
      "entry": "INTRODUCTION"
    },
    {
      "name": "What Is Creo",
      "file": "what-is-creo.md"
    },
    ...
   ]
}
```
* a `regex` entry used when files cannot be known in advance and the folder must be scanned and processed dynamically (for example documentation in the Classes folder is automatically generated by Creo):
```
{
  "TOC": [
    {
      "entry": "CLASSES"
    },
    {
      "regex": "/^(?!UI).*/"
    },
    {
      "entry": "UIKIT"
    },
    {
      "regex": "/^UI/"
    }
  ]
}
```

### Notes
You usually do not need to know these implementation details, just edit/add an md file inside a folder and then push your changes. Our script will take care of all the details. The only exception is when you add a file not previously existing in a specified folder and that folder doesn't have a regex rule. In this particular case if you want that your file appears in the documentation then you need to manually list it in the `toc.json` file.

### Examples
Every file in the examples folder is automatically appended to its main file if the example file name matches a file name previously processed by our script.

### Attachments
If you need to attach some file (like the zip project files founds in the tutorials) then prepend the special `{{github_raw_link}}` tag to its relative path. This tag will be replaced by our script with the proper GitHub link.

### Images
All images should be stored in the images folder within a subfolder with the same name of the folders that contains a `toc.json` file.

### Tutorials
All the tags used in the documentation are standard Markdown tags with the only exception of the **++N++** tag used to denote a step in the tutorial section (where **N** is a number).

### Search
Search entries are automatically generated by our script based on file name and some other information. Not all text contained in the markdown files is used, we need to find out a better stategy.

### Special considerations
If a `toc.json` file is malformed and does not contain valid JSON data than that folder is not processed. If you break something then the God of GitHub will punish you.

**Anyone can contribute to the documentation!**
