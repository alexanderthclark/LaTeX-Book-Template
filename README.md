# LaTeX Book Template

The only piece not provided here is the kdp.cls file, which helps optimize things for self publishing on Amazon. This can be found at [github.com/JenniferMack/latex-kdp](https://github.com/JenniferMack/latex-kdp).


### Value Added
The value added is just in gathering a few different things. The advantages over another template from the book class might be
* KDP class for adjusting page sizes. 
* Adding images at the beginning of each new part in the book with the epigraph package. 
* Use of the lstlistings package for inline code and code blocks.
* Some custom helper commands like `\code{}` or `\link{}{}` that simplify other commands.


Some more things in the style files could be removed for the example included. I have experimented with `\marginpar` and `\marginnote` to label code blocks with the filenames. While not demonstrated here, my solution has been to use `(*@\margintext{filename}@*)` inside the code blocks, where `(*@` and `@*)` are escape characters. `\margintext` is a custom command that uses `\marginnote` with some extra text formatting. Previously, I tried to use `\marginpar` to force all labels to the right and rotate them 90 degrees, but I was never happy with the results. 
