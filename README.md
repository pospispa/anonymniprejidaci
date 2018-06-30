# Anonymni Prejidaci website

Source code of the [anonymni prejidaci website](https://anonymniprejidaci.cz/).

## How to build the website

```
hugo server -w --renderToDisk
```
However, the above does not render future pages. To render future pages either:
```
hugo server -w --renderToDisk --buildFuture
```
or modify the `date` parameter of the future page in such a way that the page becomes a regular page.

## How to add a new page

To add a new "Akce" (blog post) issue the below command from the repo root directory:
```
hugo new --kind blog blog/<document-name>.md
```

To add a new "O nás" (docs item) issue the below command from the repo root directory:
```
hugo new --kind docs docs/<document-name>.md
```

## Potential solution to strange problems

Reset from the repo root directory:
1. Stop `hugo` server.
2. Remove all generated content: `rm -rf public/`
3. Start `hugo` server.

## Howto for the markup language used

Refer to [Kube theme for Hugo](https://themes.gohugo.io/theme/kube/) documentation.
