# Convert Jupyter Notebook To pdf
How To Convert Jupyter Notebook To pdf
Many times, after your data analysis and machine learning tasks, you would want to convert to pdf. You would require nbconvert which depends on xelatex most times (at least on linux platform) and which did not install in my Debian 12.
The following is how I was able to convert to pdf. 
1. activate your development environment
2. install nbconvert if not installed using : pip install nbconvert
3. open terminal and navigate to the location of the notebook and run the code: jupyter nbconvert file_to_be_converted.ipynb --to webpdf
4. If you encounter the following error : RuntimeError: No suitable chromium executable found on the system. Please use '--allow-chromium-download' to allow downloading one,or install it using `playwright install chromium`, run the following code. 
5. jupyter nbconvert file_to_be_converted.ipynb --to webpdf --allow-chromium-download
6. You will get a success message and the pdf will have the same name as the notebook.
Happy Coding 
