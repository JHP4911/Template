# DPhil thesis template
--------------------------

Latex template for a research progress report, a 4th year project (4YP) or a DPhil thesis for a student of the Department of Engineering Science at the University of Oxford

Requirements
--

You will need a recent version of latex installed in your system, such as Latex 2017. Install the Carlito font following the instructions for your particular operating system from the "fonts" directory. If you are using Windows system, also install the Latin Modern Math font from the "fonts" directory.

Generate PDF
--

Copy either the file sample_dphil_thesis.tex or sample_4yp_report.tex to a new file depending if you are writing a DPhil thesis or a 4YP report document respectively.

If you are using a Latex editor, configure it to run the "Lualatex" build process. If you are compiling the document manually, you would need to run the following commands:

1. lualatex  --interaction=nonstopmode project_document
2. bibtex project_document
3. makeglossaries project_document
4. lualatex  --interaction=nonstopmode project_document


You might need to run the "lualatex" command in step 4 above multiple times depending how complex is your document. Use the script "remove_latex_aux_files.sh" (in Linux or macOS) to clean the latex build.
