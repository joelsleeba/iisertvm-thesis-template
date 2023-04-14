# Before you copy and paste

  ## Why this template?

  This template is designed with only one thing in mind. The readability of the script. One of the hardest part in debugging any code, not just $LaTeX$ is squashing bugs. With a good structure to your working directory, you'll be able to read and understand what everything means and where to make changes. Without further due let us start


  ## How much $LaTeX$ you need?
  I am under the impression that you might know some $LaTeX$ scripting. Don't worry if you don't, there are plenty of YouTube videos out there. Get just the basics like how to make a simple text document, some math symbols, inline equations, block equations, aligning equations etc. [LaTeX.js](https://latex.js.org/playground.html) is an online playground which will give you a quick introduction.

  ## Where to start in this template?
  The directory is setup in a way that almost all the settings are inteh `config` directory. If you open `main.tex`, the first thing included is the `config/packages.tex`. 

  ### `config/packages.tex`
  This file imports some of the essential packages that are required. I've added what some of these packages do as comments next to them. Uncomment/add the required packages here. For more details about these packages go to [CTAN](https://www.ctan.org/) `pkg/packagename` and read the documentation there.
  
  ### `config/options.tex`
  The next thing imported by `main.tex` is `config/options.tex`. This file contains all the settings for the packages imported from `config/packages.tex`. If you want to specify further options, put all of them into this file. Refer the documentation at [CTAN](https://www.ctan.org) for specific options of the packages.

  ### `config/colors.tex`
  This file contains color settings.

  ### `config/theoremstyle.tex`
  This file contains the settings to stylize definitions and theorems for your document.

  ### `config/mathletters.tex`
  This file contains some shortcuts which helped me typeset math equations.

  ## Adding content
  The chapters of the report is supposed to be in the folder `01Chapters/`. Make a tex file for each chapter as it simplifies the content.

  ## Front Matter
  Edit the files in `00Intro/` with your details.

  ## Citations and References
  Cite whatever you want with `\autocite` and refer things with `\autoref`. Its way better than `\ref`. Look at the code to see what I mean.

  The bibliography file is set to `02End/math.bib`, using `bibsource` in line 8 of `main.tex`. Edit the `.bib` file adding your citations. The `citationstyle` can also be changed. Refer `biblatex` documentation for this. 

  Remember to run `biber` if you are working in your local system and not [Overleaf](https://www.overleaf.com).
