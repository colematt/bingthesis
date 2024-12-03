<!-- vscode-markdown-toc -->
* [Purpose](#Purpose)
* [Installation](#Installation)
* [Building the Sample Thesis](#BuildingtheSampleThesis)
* [Licensing](#Licensing)
	* [How You Can Help](#HowYouCanHelp)
* [References](#References)

<!-- vscode-markdown-toc-config
	numbering=false
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

# bingthesis
A LaTeX thesis and dissertation template for Binghamton University

## <a name='Purpose'></a>Purpose

When I wrote my dissertation in 2024, I found that there were a few challenges:

- The Graduate School is under the impression that most PhD candidates are using Microsoft Word. At least in the STEM fields, this is not correct. We've been writing conference papers and journal articles in LaTeX, and these manuscripts form a programmatic line of research that becomes our dissertation or thesis. Rewriting in Word is out of the question.
- There is no official LaTeX style file, therefore most people are reusing a [Mathematics Department template](https://www2.math.binghamton.edu/p/gd/dissertation) from the mid-aughts with a lot of fragile, obsolete LaTeX idioms and opinionated macros that will conflict with other departments' style guides. 
    - I tried to write a style file rather than a template that captured only the Graduate School's requirements, deferring as many style choices to your preamble as possible. 
    - The included template is simply a recreation of the Graduate School's own sample, illustrating how to use the style file, rather than a requirement to get the right style.
- Most graduate students are not "TeX-nicians", and can't/shouldn't invest the time to learn to write their own style file. Besides, you get no credit for reinvention.

## <a name='Installation'></a>Installation

If you already have a work in progress written in LaTeX, it is sufficient to:

1. Put **bingthesis.sty** in the same directory as your root file
2. Use a `\usepackage{bingthesis}` directive in your document preamble before any other `\usepackage{}` directives

Otherwise, you can start writing your dissertation by modifying the sample dissertation included in this repository.

## <a name='BuildingtheSampleThesis'></a>Building the Sample Thesis

Build the sample dissertation in whichever method is most compatible with your existing workflow.

- Uploading this entire repository to a blank Overleaf project and let it build. Overleaf has all required packages globally available except **bingthesis.sty**.
- Build this repository using a LaTeX IDE such as TeXStudio or Texifier. For the former, you will need to change your bibliography engine from Bibtex to Biber.
- Build with a build tool such as `latexmk` (included with most LaTeX distributions) or [`rubber`](https://gitlab.com/latex-rubber/rubber/). Use **main.tex** as the root document.

## <a name='Licensing'></a>Licensing

The[GNU Public License (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.html) is a [free software license](https://www.gnu.org/philosophy/free-sw.en.html).
Therefore you have the right to use this repository's code freely while preparing your dissertation.
The Graduate School's [Guidance for Writing and Formatting Your Thesis or Dissertation](https://drive.google.com/file/d/1yx6AU93JfRZ-AdCzgGcTfemUZ1QhvvAX/view?pli=1) requires a preface statement to the effect of "_All relevant permissions have been granted by the corresponding author(s) for the use of copyrighted materials._"
For purposes of that affirmation, consider that permission granted by virtue of this repository's [LICENSE](https://github.com/colematt/bingthesis/blob/main/LICENSE).

### <a name='HowYouCanHelp'></a>How You Can Help
Explicit acknowledgement within your dissertation or thesis isn't required, although you can still help by doing one or more of the following:

- Fork and/or star this repository. Doing so enhances its prominence in search engine results.
- Let the Graduate School, your Department, and your Dissertation/Thesis Supervisor know that you wanted a template, but could only find a sample PDF without any of its source code.
- Contribute improvements by either opening a new issue (and using one or more label to describe it), or even better submitting a change via pull request.
- Leave the license statement in [bingthesis.sty](https://github.com/colematt/bingthesis/blob/main/bingthesis.sty) intact as a way of pointing future reusers towards this repository.

## <a name='References'></a>References

- [Guidelines for Preparing or Submitting a Thesis or Dissertation](https://www.binghamton.edu/grad-school/policies-and-procedures/manual/thesis-dissertation.html)
- [Thesis/Dissertation Sample (.pdf)](https://www.binghamton.edu/grad-school/pdf/thesis_dissertation_template.pdf)
- [Thesis/Dissertation Submission](https://www.binghamton.edu/grad-school/academic-support/submit-thesis-dissertation.html)
- [Guidance for Writing and Formatting Your Thesis or Dissertation](https://drive.google.com/file/d/1yx6AU93JfRZ-AdCzgGcTfemUZ1QhvvAX/view?pli=1)
