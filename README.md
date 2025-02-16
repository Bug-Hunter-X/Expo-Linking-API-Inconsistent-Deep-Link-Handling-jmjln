# Expo Linking API Inconsistent Deep Link Handling

This repository demonstrates a bug in Expo's `Linking` API where deep link events are not consistently handled when the app is in the background.  The `Linking.addEventListener` sometimes fails to trigger, leading to missed deep link data.

The `deepLinkBug.js` file shows the problematic implementation, and `deepLinkSolution.js` provides a workaround that uses a combination of event listeners and a background service to ensure deep links are always processed.

This issue is particularly relevant for apps that rely heavily on deep links for various functionalities such as sharing, login, or content routing.