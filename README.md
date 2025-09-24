# A Simple Email Signature Builder

Made with [Svelte](https://svelte.dev).

## Features

- Update name, title, and phone via form
- Button to copy signature for pasting into email client
- Name, title, and phone saved to URL query strings so can be bookmarked
- Very awful HTML should (hopefully) work on all clients.

## Screenshot

<img width="537" height="662" alt="image" src="https://github.com/user-attachments/assets/e88b55f1-5f58-4a4b-a41d-f3b21b196e3d" />

## Installation

- In `/public` make sure you have your logo and preferred social media icons (Instagram, YouTube, LinkedIn, and Facebook are included)
- In `Signature.svelte` edit `logoUrl` and `links`
- Update the `--base=/sigmaker` parameter to the build script in `packages.json` (default assumes you will copy files to a sub-directory called `sigmaker` on your webserver, eg. http://example.com/sigmaker/).
- To deploy run `yarn build` and then copy all files in `/dist` to a webserver

