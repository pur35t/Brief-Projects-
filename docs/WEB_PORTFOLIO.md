# Updating the visual portfolio

The website is `index.html` at the repository root. It uses the existing `assets/images` folder, so there is no build step or dependency installation.

## Edit a project

Open `index.html` and search for `const PORTFOLIO_DATA = {`. Edit the project title, summary, status, tags, bullets, images, and evidence links in that object. Most content changes do not require editing the rendering functions.

To add a supporting project, copy an existing object with `featured: false`. Give it a unique id, add its images, and link its documentation. For a featured photograph project, use `media: 'lead-photo'` and set `lead` to an image path. Update the project jump links if you add a new featured project.

## Add a photo

Upload the file into `assets/images/`, then add its path to the project's `images` array. Prefer a descriptive filename, such as `assets/images/balancing-robot-first-test.jpg`. Photos open in a full-size image viewer. Galleries show a few images first and can expand to show the rest.

Keep project status and team attribution accurate. The ~98% chess-camera result is an informal team observation. The speaker is a design proposal.

## Publish on GitHub Pages

After merging the website change, open the repository Settings, select Pages, choose Deploy from a branch, and select `main` with `/ (root)`. GitHub will show the published URL when deployment completes. The page works from a repository subpath because its local assets use relative paths.

The source change does not enable GitHub Pages or change repository settings. The public website links to the existing public portfolio PDF. It does not publish the separate resume attachment.

## Share a single HTML file

The standalone edition embeds its source images and the owner's resume PDF. Open that file in a browser to inspect it without an adjacent asset folder. GitHub links and video playback still require internet access.

## Video

The chess project links to `https://www.youtube.com/watch?v=CqR65Nzltz0` and has an embedded player that loads on click. No extracted video frames are included: access to the video was blocked during this update.
