# Welcome to Discover three.js!

This is the public repo for the book [Discover three.js](https://discoverthreejs.com/).

Pull requests are welcome, especially for:

* Keeping the book up to date with new three.js releases.
* Errata in the text or code examples.
* Any other bugs, browsers, or CSS issues.

For larger contributions, please get in touch with on lewy@discoverthreejs.com before making changes.

## Developer Guide

To build and view the book.

Prerequisites: Node.js

1. Clone or download the repo
2. Run `npm install`
3. Create symlink for the static/examples folder into markdown/assets (This is required since Hugo.readFile cannot access files outside the /markdown folder)
4. Run `npm start` and open your browser to `http://localhost:8080/`
