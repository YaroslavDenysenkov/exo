---
groups:
  - tool_linux
---


```cardlink
url: https://github.com/mkaz/termgraph
title: "GitHub - mkaz/termgraph: A Python command-line and library that draws basic graphs in the terminal"
description: "A Python command-line and library that draws basic graphs in the terminal - mkaz/termgraph"
host: github.com
favicon: https://github.githubassets.com/favicons/favicon.svg
image: https://opengraph.githubassets.com/c8bb3bd98df79693ff86021421b460b81ac5370230d23034f038767c8e116b1d/mkaz/termgraph
```

*pip install termgraph*
*pipx install termgraph*

*du -d 1 | awk '{print $2, $1}' | termgraph*


```bash
du ./../ -m -d 1 | grep -v "\.\.$" | sort -nr | awk -F'\t' '{
  size=$1; 
  split($2, path, "/"); name=path[length(path)]; # Get just the folder name, not the whole path
  if (size > 500) print name, size, 0, 0;
  else if (size > 100) print name, 0, size, 0;
  else print name, 0, 0, size;
}' | termgraph --color red yellow green --stacked
```



- [ ] Grok python virtual env, and pip vs pipx


