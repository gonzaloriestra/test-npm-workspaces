Steps to reproduce:
- `git clone https://github.com/gonzaloriestra/test-npm-workspaces.git`
- `npm i`
- `npm run dev -- --skip-dependencies-installation`
- Open "App home", install the app and check that it works
- Open "product subscription", go to to "Add purchase option" - "Select existing option", and it crashes

Error in Chrome dev console:
```
p_shared_components_UIExtensions_shared_UIExtensionsContent_UIExtensionsContent_tsx-app_sha-21d79e-277d5e7eecb6d01e.js:1 Uncaught (in promise) Error: Invalid hook call. Hooks can only be called inside of the body of a function component. This could happen for one of the following reasons:
1. You might have mismatching versions of React and the renderer (such as React DOM)
2. You might be breaking the Rules of Hooks
3. You might have more than one copy of React in the same app
See https://reactjs.org/link/invalid-hook-call for tips about how to debug and fix this problem.
    at resolveDispatcher (main.js?lastUpdated=1682524063823:17562:23)
    at useContext3 (main.js?lastUpdated=1682524063823:17568:30)
    at useExtensionApi (main.js?lastUpdated=1682524063823:19315:46)
    at App (main.js?lastUpdated=1682524063823:19356:32)
    at renderWithHooks (main.js?lastUpdated=1682524063823:7150:28)
    at mountIndeterminateComponent (main.js?lastUpdated=1682524063823:9326:23)
    at beginWork (main.js?lastUpdated=1682524063823:10155:24)
    at Object.invokeGuardedCallbackProd (main.js?lastUpdated=1682524063823:11157:20)
    at invokeGuardedCallback (main.js?lastUpdated=1682524063823:11244:41)
    at beginWork$1 (main.js?lastUpdated=1682524063823:14123:17)
(
```
