# picolisp-onedoc-html
## Concatenate PicoLisp reference and tutorial files into one file

Sometimes one may want to have all the PicoLisp reference and tutorial files available as one big
HTML file. To concatenate lots of files may be trivial, however, adjusting all the internal links
turned out to be a challenge. Now it seems to work.

One thing that remains to be fixed, is the JavaScript based buttons "Sort Words Alphabetically".
They end up side by side in the main Function Reference, and they don't work. It's probably best to
solve this in the original files, but I have not found the right way to do it yet.

Before you run the script, you should
```
cd picoLisp/doc/
```
Then do
```
pil pathTo/convConcat.l pathTo/output.html
```
The resulting file "output.html" now contains all references and tutorials, but you need to supply
a header and some "footer". You may copy/paste these parts from the file src/head-foot.html.

To get a nice working layout I suggest you use the file src/doc.css. This CSS can certainly be
improved, but for now it should be OK. It may also work OK on a tablet.

An example of a complete concatenated file can be seen here:

http://folk.uio.no/jkleiser/pico/one/one.html
