---
title: "quartz - github deploy error"
tags:
description: 
aliases: 
date: "2025-07-19T13:13:17"
---

.

오랜만에 써봤는데, 페이지가 업데이트가 안된다.

다음과 같은 github action 에러가 발생했다.  
quartz 디렉토리 안에 있는 `.github/workflows/deploy.yml` 를 다음과 같이 수정하여 에러를 고쳤다.

---
### build error 1

> **build**  
> This request has been automatically failed because it uses a deprecated version of `actions/upload-artifact: v3`. Learn more: [https://github.blog/changelog/2024-04-16-deprecation-notice-v3-of-the-artifact-actions/](https://github.blog/changelog/2024-04-16-deprecation-notice-v3-of-the-artifact-actions/)

2025년 1월부터 `actions/upload-artifact: v4` 를 써야한다.

```yaml
name: Deploy Quartz site to GitHub Pages

on:
  push:
    branches:
      - v4

permissions:
  contents: read
  pages: write
  id-token: write

concurrency:
  group: "pages"
  cancel-in-progress: false

jobs:
  build:
    runs-on: ubuntu-22.04
    steps:
      - uses: actions/checkout@v4 # Changed from v3 to v4
        with:
          fetch-depth: 0 # Fetch all history for git info
      - uses: actions/setup-node@v4 # Changed from v3 to v4
        with:
          node-version: 18.14
      - name: Install Dependencies
        run: npm ci
      - name: Build Quartz
        run: npx quartz build
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3 # Changed from v2 to v3
        with:
          path: public

  deploy:
    needs: build
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4 # Changed from v2 to v4
```

---

### build error 2


> Run npm ci  
> npm ci  
> 
> shell: /usr/bin/bash -e {0}  
> npm ERR! code EBADENGINE  
> npm ERR! engine Unsupported engine  
> npm ERR! engine Not compatible with your version of node/npm: @jackyzha0/quartz@4.5.1  
> npm ERR! notsup Not compatible with your version of node/npm: @jackyzha0/quartz@4.5.1  
> npm ERR! notsup Required: {"npm":">=10.9.2","node":">=22"}  
> npm ERR! notsup Actual:   {"npm":"9.5.0","node":"v18.14.2"}  
> npm ERR! A complete log of this run can be found in:  
> npm ERR!     /home/runner/.npm/_logs/2025-07-19T03_56_21_006Z-debug-0.log  
> Error: Process completed with exit code 1.  

quartz 4.5.1 로 업데이트해서 그런지 node 22.x 버전으로 맞춰야 한다.

```yaml
jobs:
  build:
    runs-on: ubuntu-22.04
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0 # Fetch all history for git info
      - uses: actions/setup-node@v4
        with:
          node-version: 22.x # Changed to Node.js 22.x (or 22)
      - name: Install Dependencies
        run: npm ci
      - name: Build Quartz
        run: npx quartz build
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: public
```



.

