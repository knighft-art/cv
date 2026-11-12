# Han-Yup Yum, Ph.D.

Personal academic curriculum vitae site for Han-Yup Yum, Ph.D. This is not a ChamomileGrey project.

**Live site:** https://hanyupyum-founder.chamomilegrey.workers.dev

The PDF is the source of truth. The page does not restate the CV. It offers a browser view and a download of that same file. Do not retypeset, rewrite, or replace the PDF with HTML body text.

## What is published

| URL | File | How it is served |
| --- | --- | --- |
| `/` | `public/index.html` | Heading, view, and download |
| `/cv.pdf` | `public/cv.pdf` | `application/pdf`, inline |
| `/Han-Yup_Yum_Ph.D._CV.pdf` | `public/Han-Yup_Yum_Ph.D._CV.pdf` | `application/pdf`, download |

`public/cv.pdf` and `public/Han-Yup_Yum_Ph.D._CV.pdf` are byte-for-byte copies of the official CV. When the CV changes, replace both files with the same new PDF.

On a desktop browser the page embeds `/cv.pdf`. Download stays available on every screen, which is the reliable way to read the CV on a phone.

## Deploy

This repository is a Cloudflare Workers static-asset site (not Pages). The Worker name is `hanyupyum-founder`, `workers_dev` is enabled, and there are no bindings, secrets, or telemetry. The public address is https://hanyupyum-founder.chamomilegrey.workers.dev.

After merging to `main`, publish from a checkout of that branch:

```sh
npx wrangler deploy
```

Deployment is manual. This repo does not configure GitHub Actions.

Local preview:

```sh
npm install
npm run dev
```

## Rights

All rights reserved.
