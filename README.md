# Bug Report

If a project contains symbolic links (symlinks), it cannot be successfully fetched by the `zig fetch` command.

Here is a minimal example: a project that includes a symlink pointing to the `README` file. When you attempt to fetch it with `zig fetch`, the following error occurs:

```
error: unable to hash 'README': Unexpected
```

This issue may prove fatal to compatibility with the C/C++ ecosystem.