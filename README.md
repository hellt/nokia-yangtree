# Nokia YANGtree
Nokia YANGtree repo contains the most common YANG output formats generated from the original [Nokia 7x50 YANG models](https://github.com/nokia/7x50_YangModels) source. The provided output formats (generated with pyang) are:

- text based `tree` version. `.txt` extension
- XML (aka YIN) notation with `.xml` extension
- HTML file with `.html` extension

Additionally, this repo provides the XPATH path collection (`*paths.txt|html`) that enables you to easily navigate and search through the YANG model paths.

## 1 Releases
The repo structure leverages git [tags](https://github.com/hellt/nokia-yangtree/tags). Each tag points to a file collection generated for a specific Nokia 7x50 release. To browse the artifacts for a certain SR OS release, select the corresponding tag as demonstrated:

> ![select_tag](https://gitlab.com/rdodin/pics/-/wikis/uploads/8e9e7582ff6b90fef02c9fd529d84303/CleanShot_2020-05-19_at_14.28.31.gif)


## 2 YANG browser
The following web pages have been generated for you to easily navigate SR OS YANG models:

* Nokia `configuration` datastore
  * [HTML tree](https://rdodin.gitlab.io/nokia-yangtree-srv/sros_21.2.r1-nokia-conf-combined.html)
  * [Path browser](https://rdodin.gitlab.io/nokia-yangtree-srv/sros_21.2.r1-nokia-conf-combined-paths.html)
* Nokia `state` datastore
  * [HTML tree](https://rdodin.gitlab.io/nokia-yangtree-srv/sros_21.2.r1-nokia-state-combined.html)
  * [Path browser](https://rdodin.gitlab.io/nokia-yangtree-srv/sros_21.2.r1-nokia-state-combined-paths.html)

> Note: due to the substantial size of the HTML documents it might take a while to load them.

Read more about the YANG browser capabilities [here](https://netdevops.me/2020/nokia-yang-tree/).

## 3 Download
There are several ways to download the outputs for a specific release. The below examples will assume the `sros_21.2.r1` release is in question.

### 3.1 Clone with git
If git is installed it is possible to clone the artifacts for a specific tag with the following command:
```
git clone -b sros_21.2.r1 --depth 1 https://github.com/hellt/nokia-yangtree
```

### 3.2 Archives
It is possible to download the whole outputs collection for a specific release in the `zip` or `tgz` containers.

The github `releases`(https://github.com/hellt/nokia-yangtree/releases) page contains the direct links to those archives. If needed, the download link can be programmatically concatenated using the following rule:

**for zip**
`https://github.com/hellt/nokia-yangtree/archive/` + `tag_name` + `zip`

**for tar.gz**
`https://github.com/hellt/nokia-yangtree/archive/` + `tag_name` + `tar.gz`

Here are the direct links to download `sros_21.2.r1` models outputs in the respective containers:
- [sros_21.2.r1.zip](https://github.com/hellt/nokia-yangtree/archive/sros_21.2.r1.zip)
- [sros_21.2.r1.tar.gz](https://github.com/hellt/nokia-yangtree/archive/sros_21.2.r1.tar.gz)
