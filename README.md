# Steps to recreate Parcel HMR issue

1. Clone this repo
2. yarn install
3. yarn dev
4. Open in Chrome on http://localhost:1234
5. Open browser console
6. Make a change to the JSX in src/index.html
7. See the console say "Console was cleared"
8. Page will not replace the content you change, or reload

# Steps to fix HMR issue

1. Open src/index.html and remove the script tag on the <head>
2. Refresh browser on http://localhost:1234
3. HMR should be working again
