# 10k IPs

[Demo](https://bennyboy.tech/ipisp)

Data visualization of IP (Internet Protocol) addresses and ISPs (Internet Service Providers) in the UAE. This project aims to provide a data-driven insight into corporate ownership and control over the UAE's Internet, as well as provoke discussions about net neutrality, security, and communication. Data was gathered from [Shodan](https://shodan.io) and displayed using [Sigma js](http://sigmajs.org).

## Modifications

If you wish to run/modify the code yourself, then this section is for you.

Requirements:
- Python 3+
- Jupyter Notebook
  - `pip install jupyter notebook`
- Python modules: shodan, matplotlib, networkx, pygraphviz
  - `pip install shodan matplotlib networkx pygraphviz`
- Shodan account
  - depending on the amount of data you wish to gather, you may need a membership
  
To gather your own data, run this command within the project's working directory (modify parameters to fit your own needs):
```
shodan download --limit 15000 isp10k country:AE
```

Then run `main.ipynb` in Jupyter Notebook to generate the visualization.

## Credits

Made in collaboration with Leo El-azhab and Mai Khaled. Distributable under MIT License.
