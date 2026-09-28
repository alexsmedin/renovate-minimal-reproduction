# 46408

## Current behavior

Renovate makes API requests to `/tfs/Collection/_apis/Location`, `/tfs/Collection/_apis/git` and `/tfs/Collection/_apis/ResourceAreas` that fail randomly with timeout errors. Other requests are working and it is able to create pull requests in azure devops server.

## Expected behavior

The API requests should succeed, or the timeout/concurrency be configurable to make it able to do so. 

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/46408
