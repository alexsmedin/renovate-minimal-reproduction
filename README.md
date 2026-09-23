# minimal-reproduction-template

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).

Then replace the current `h1` with the Renovate Issue/Discussion number.

## Current behavior

Renovate makes API requests to `/tfs/Collection/_apis/Location` and `/tfs/Collection/_apis/git`, which fails due to the endpoints not existing. Renovate reports API timeouts, curl to the same endpoints returns 404. Other requests are working and it is able to create pull requests in azure devops server.

## Expected behavior

The API requests should be normalized and directed to `/tfs/_apis/Location` and `/tfs/_apis/git` (without the collection name), but the repositories discovered under `/tfs/Collection/`.

## Link to the Renovate issue or Discussion

Put your link to the Renovate issue or Discussion here.
