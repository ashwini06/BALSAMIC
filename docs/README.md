### Build BALSAMIC doc locally

Create a conda environment:

```
conda create -n balsamic_doc -c bioconda -c conda-forge python=3.6 pip
conda activate balsamic_doc
```

Install Sphinx and extensions:
 
```
cd docs
pip install -r requirements.txt 
```

Build docs:

```
sphinx-build -T -E -b html -d _build/doctrees-readthedocs -D language=en . _build/html
```

View docs (`open` or similar command from your OS):

```
open _build/html/index.html 
```
