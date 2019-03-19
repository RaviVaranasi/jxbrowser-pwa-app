# Steps to reproduce problem

1. Run `npm install -g serve`
2. Run `npm run build`
3. Run `serve -s build`
4. Open `http://localhost:5000` from jxbrowser.
5. Should see `Error during service worker registration: DOMException: Failed to register a ServiceWorker: No URL is associated with the caller's document.` error in console within jxbrowser remote debugging window.


# Setup
1. Ran `npx create-react-app jxbrowser-create-react-app`
2. Open `index.js` and changed from `service.unregister()` to `service.register`
3. Followed instructions above after this.