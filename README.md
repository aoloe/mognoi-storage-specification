mognoi-storage-specification
============================

The specification of the storage for the Mognoi project.

- Add a two letter language code for each translated file, before the extension and prefixe by a dash (as in `README-de.md`). In
- there is a .sla per language
- the content is created in .md files that are manually imported into the .sla
- the images are also manually inserted
- each section has its own folder that contains, the text for the chapter in a .md file (each translation in one file), the images to be published both in web and print resolution (and eventually translated), the resources used to create the images (in a `resource/` directory), a README.md file with notes about the section and a list of changes and authors per language.
- the section's folders are called by the english chapter title, a dash and the english section title. the title may be shortened.
- images are called
  - `web-name_of_the_image.png` or
  - `print-name_of_the_image.png`
  depending on their size.  
  if the image contains language dependent content, you will add:
  - `web-name_of_the_image-fr.png`
- if you want to add text or vectors to an image, create an SVG and draw them in there.
  - bitmaps should be on layers named `web` and `print`
  - all language specific elements should go into a layer named after the language (fr, en, ...)

#TODO
- remove all typographic signs (’, «) and replace them in the sources with the normal ones.
- remove the spaces before the :;... (they can be correctly readded when importing into scribus. or add them as non breaking space instead of normal spaces)


# TOOLS

- html to markdown: <http://html2markdown.com/>
