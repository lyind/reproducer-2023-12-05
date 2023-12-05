## Reproducer for Hugo/Goldmark issue

Render with Hugo (tested with v0.120.4, v0.121.0 and main) in this directory:
```
hugo --verbose --cleanDestinationDir --destination public
```

If the issue occurs, one should see an error containing this message:
```
Error: error building site: render: failed to render pages: render of "term" failed: template: _internal/_default/rss.xml:67:22: executing "_internal/_default/rss.xml" at <.Summary>: error calling Summary: runtime error: index out of range [32] with length 20
```
