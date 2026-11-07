# WebDesk

A free, static GitHub Pages demo for consent-based browser screen sharing.

## What it does
- Uses the browser's built-in screen-sharing permission prompt.
- Streams the selected screen to another browser using WebRTC.
- Uses manual offer/answer code exchange, so no signalling server is needed.

## What it does NOT do
- No remote mouse or keyboard control.
- No unattended access.
- No remote file browsing or file transfer.
- No guarantee that every network will allow a direct peer-to-peer connection. Some networks require a TURN relay server, which is not included.

## Publish with GitHub Pages
1. Sign in to GitHub and create a new **public** repository named `webdesk`.
2. Upload `index.html` to the repository's root (and optionally this README).
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. Open the HTTPS URL shown on the Pages settings screen.

## Use it
1. Both people open the published HTTPS URL in a recent Chrome or Edge browser.
2. The sharing person selects **I am sharing**, clicks **Choose screen**, and chooses a screen/window in the browser prompt.
3. They send the generated offer code privately to the viewer.
4. The viewer selects **I am watching**, pastes the offer, clicks **Create answer**, and sends the answer code back.
5. The sharing person pastes the answer and clicks **Connect to viewer**.

The sharing person can stop sharing from the browser's sharing indicator or the page's Stop sharing button.

## Security notes
Only share with someone you trust. Treat offer/answer codes as private connection information. This is a learning/demo project, not a hardened remote-support service.
