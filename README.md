# parcellscope website

The public front page for parcellscope, served by GitHub Pages at
**https://drnjain.github.io/parcellscope-website/**.

It describes the app for visitors and sends them to the app's sign-in page with
**Access App** (`https://parcellscope.tail1da2ea.ts.net/`). It holds no participant data and
nothing about how the app works behind the scenes. The app's own code lives in a separate,
private repository.

| File | What it is |
|---|---|
| `index.html` | the page: all text and the links |
| `site.css` | colours, fonts and layout (phone to wide monitor) |
| `brain.js` | the rotating 3D brain in the top section; drag to turn it, double-click to reset |
| `favicon.svg` | the browser-tab icon |
| `.nojekyll` | tells GitHub Pages to serve the files as they are |

Plain static files with no build step. A change pushed to `main` is live a minute or two later.

To change the app address, edit the `href="https://parcellscope.tail1da2ea.ts.net/"` lines in
`index.html` (there are three Access App buttons).

The brain shape comes from FSL's MNI152 1 mm template (every surface voxel) and the
Harvard-Oxford subcortical atlas (thalamus, caudate, putamen, pallidum, hippocampus,
amygdala, accumbens), stored in `brain.js` as whole-millimetre coordinates. These are public
standard templates, credited in the page footer.
