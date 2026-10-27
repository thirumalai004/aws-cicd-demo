# AWS CI/CD Demo

This project is a simple static website that demonstrates a basic AWS CodeBuild pipeline for packaging and publishing a web page.

## Project structure

- `index.html` – the static site content
- `buildspec.yml` – build specification used by AWS CodeBuild

## What the pipeline does

The build process:

1. Validates that `index.html` exists
2. Creates a `dist` directory
3. Copies the app files into `dist`
4. Publishes the `dist` folder as the build artifact

## Preview locally

Open `index.html` in a browser or serve the folder with a simple local web server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Notes

This demo is intentionally minimal and is meant to show how a static site can be packaged with AWS CI/CD tooling.
