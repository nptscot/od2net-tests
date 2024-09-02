# Demo of od2net


The in this repo is intended to demonstrate how to use
[`od2net`](https://github.com/Urban-Analytics-Technology-Platform/od2net)
to generate route networks and to compare the workflow, and results,
with the R-based approach currently used in the NPT project.

# od2net minimum example

The following is based on [`od2net`’s
docs](https://github.com/Urban-Analytics-Technology-Platform/od2net/blob/main/docs/tutorial_examples.md#running-the-edinburgh-example)
and the code in the examples/edinburgh folder.

We will run the code on a computer with Ubuntu 22.04 after running the
setup outlined in the link above.

``` {bash}
#| eval: false
#| echo: false
sudo apt install osmium-tool
```

``` {bash}
#| eval: false
gh repo clone Urban-Analytics-Technology-Platform/od2net
# Copy the example to this folder:
cp -r od2net/examples/edinburgh/* .
cp -r od2net/
python3 setup.py
```

``` {bash}
```

\`\`\`
