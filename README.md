[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/ULL-MII-SYTWS-2122/hello-js-action-alu0100898293)

# hello-js-action-alu0100898293

This action create a comment whenever a pull request is opened on our repository and add labels depending on the file types changed. The comment will contain a summary of the changes introduced in the pull request.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

### `owner`

**Required** The owner of the repository

### `repo`
    
**Required** The name of the repository

### `pr_number`

**Required** The number of the pull request

### `token`

**Required** The token to use to access the GitHub API

## Example usage

uses: ULL-MII-SYTWS-2122/hello-js-action-alu0100898293@optional
with:
    owner: ${{ github.repository_owner }}
    repo: ${{ github.event.repository.name }}
    pr_number: ${{ github.event.number }}
    token: ${{ secrets.GITHUB_TOKEN }}