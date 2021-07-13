- Clean brew cache
  - brew cleanup
  ```
  If --prune=days is specified, remove all cache files older than days.

  If --dry-run or -n is passed, show what would be removed, but do not actually remove anything.

  If -s is passed, scrub the cache, removing downloads for even the latest versions of formulae. Note downloads for any installed formulae will still not be deleted. If you want to delete those too: rm -rf $(brew --cache)
  ```

- Update brew
  - brew update

- Upgrade brew
  - brew upgrade 
