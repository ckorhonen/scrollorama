# Repository guide

`js/jquery.scrollorama.js` is the scroll-animation plugin; `index.html` contains the demo and animation setup; `css/` styles it. The demo loads vendored jQuery 1.7.1 and Lettering 0.6.1. Preserve those dependencies and the existing visual identity unless a change explicitly requires otherwise.

There is no package manifest, dependency installation, build, lint, automated test, or CI configuration. Open `index.html` in a browser or use a disposable local static server. With Node available, `node --check js/jquery.scrollorama.js` checks plugin syntax only. For animation changes, inspect scrolling in both directions, block transitions, intermediate states, and the browser console; screenshots at multiple positions help verify the result. Do not claim browser behavior from syntax checks alone.

Check `git status --short`, preserve unrelated changes, and finish authorized local edits through focused verification and repair. Make ordinary reversible choices directly; do not introduce a build system to validate a small plugin edit. External publishing requires task authorization. If a browser is unavailable, report the missing visual check and continue independent source checks. For prose-only changes, verify references and run `git diff --check`; close with changed paths, actual checks/results, and remaining risks.
