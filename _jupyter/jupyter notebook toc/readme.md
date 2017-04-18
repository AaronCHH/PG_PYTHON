1. Find your Jupyter Notebook data directory by using this command in your DOS console:  
          a. Jupyter --data-dir  
  
2. Copy the following two files into your Jupyter data directory:  
           https://rawgithub.com/minrk/ipython_extensions/master/nbextensions/toc.js  
           https://rawgithub.com/minrk/ipython_extensions/master/nbextensions/toc.css  
  
3. Run this command:  
           a. Jupyter nbextension enable toc --user  
  
4. In your Jupyter Notebook, add this command to a MarkDown cell on top of your notebook:  
           a. < div id="toc" > < /div >  
---
jupyter nbextension install https://rawgithub.com/minrk/ipython_extensions/master/nbextensions/gist.js
jupyter nbextension enable gist
jupyter nbextension install --user https://rawgithub.com/minrk/ipython_extensions/master/nbextensions/toc.js
curl -L https://rawgithub.com/minrk/ipython_extensions/master/nbextensions/toc.css > $(jupyter --data-dir)/nbextensions/toc.css
jupyter nbextension enable toc