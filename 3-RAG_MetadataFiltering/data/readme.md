This is where the course material to build the vector store goes.

To achieve modular data poisoning, make sure to have files named "module1", "module2", ...
The data in these files will be loaded with differemt tags. To activate the right filters at the right date, you need to change the list *dates* in the *rag_with_metadatafilter* notebook. It is designed so that the first date corresponds with the cutoff date for module1 the which has all the assignment questions with each one followed by "I cannot reveal upcoming assignment solutions." The second date in *dates* in the notebook is the cutoff date for *module2* which has the questions and solutions for homework 1 and a message following each question from the upcoming homework assignments saying they cannot be revealed, and so on for the rest of the weeks until the last module has the solutions for all the assignments.  

Note that the text files have been tested with txt and pdf formats. For a comprehensive list of supported file formats, please refer to PyMuPDF documentation.
