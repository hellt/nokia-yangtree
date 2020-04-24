# Nokia YANGtree
Nokia YANGtree repo contains the most common YANG output formats generated from the original [Nokia 7x50 YANG models](https://github.com/nokia/7x50_YangModels) source. The supported output formats (generated with pyang) are:

- text based `tree` version. `.txt` extension
- XML (aka YIN) notation with `.xml` extension
- HTML file with `.html` extension

## 1 Releases
The repo structure leverages git [tags](https://github.com/hellt/nokia-yangtree/tags). Each tag points to a file collection generated for a specific Nokia 7x50 release. To select a SR OS go to the tags section as displayed:

![select_tag](https://gitlab.com/rdodin/pics/-/wikis/uploads/43cc6afb381976990c18de526fe906e6/yangtree.gif)

## 2 Download
There are several ways to download the outputs for a specific release. The below examples will assume the `sros_20.2.r2` release is in question.

### 2.1 Clone with git
If git is installed it is possible to clone the artifacts for a specific tag with the following command:
```
git clone -b sros_20.2.r2 --depth 1 https://github.com/hellt/nokia-yangtree
```

### 2.2 Archives
It is possible to download the whole outputs collection for a specific release in the `zip` or `tgz` containers.

The github `releases`(https://github.com/hellt/nokia-yangtree/releases) page contains the direct links to those archives. If needed, the download link can be programmatically concatenated using the following rule:

**for zip**
`https://github.com/hellt/nokia-yangtree/archive/` + `tag_name` + `zip`

**for tar.gz**
`https://github.com/hellt/nokia-yangtree/archive/` + `tag_name` + `tar.gz`

Here are the direct links to download `sros_20.2.r2` models outputs in the respective containers:
- [sros_20.2.r2.zip](https://github.com/hellt/nokia-yangtree/archive/sros_20.2.r2.zip)
- [sros_20.2.r2.tar.gz](https://github.com/hellt/nokia-yangtree/archive/sros_20.2.r2.tar.gz)

## 3 HTML preview
The HTML representation of the YANG models can be viewed in a browser without downloading the files. Prepend the path to the file with `http://htmlpreview.github.io/?` to have a served HTML file.

For your convenience, each tagged release comes with the direct urls:

- [nokia-conf-combined](http://htmlpreview.github.io/?https://github.com/hellt/nokia-yangtree/blob/sros_20.2.r2/sros_20.2.r2-nokia-conf-combined.html)
- [nokia-state-combined](http://htmlpreview.github.io/?https://github.com/hellt/nokia-yangtree/blob/sros_20.2.r2/sros_20.2.r2-nokia-state-combined.html)