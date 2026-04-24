# Esports Careers Webpage

This project is a static one-page site built for a school multimodal assignment. It is designed to deploy cleanly on Cloudflare Pages with no build step.

## Files

- `index.html`: page structure and content
- `styles.css`: design system, layout, and responsive styling
- `app.js`: section-aware navigation highlighting

## Cloudflare Pages setup

These steps match Cloudflare Pages' current Git-based static HTML flow from the official docs:

1. Put these files in a GitHub or GitLab repository.
2. In the Cloudflare dashboard, open **Workers & Pages**.
3. Select **Create application**.
4. Select the **Pages** tab.
5. Choose **Import an existing Git repository**.
6. Select your repository and choose **Begin setup**.
7. Use these build settings:
   - Production branch: `main`
   - Build command: `exit 0`
   - Build output directory: `/` or `.` if Cloudflare asks for a relative root path
8. Start the deployment. Cloudflare will publish the site to a `*.pages.dev` URL.

## Notes

- The homepage starts at `index.html`, which Cloudflare Pages expects for the root URL.
- Google Fonts are loaded from the browser at runtime, so you do not need a build tool.
- The visual panels for the "image" areas are stylized backgrounds inspired by your search prompts, which keeps the project self-contained and easy to deploy.

## Official references

- Cloudflare Pages getting started: https://developers.cloudflare.com/pages/get-started/
- Cloudflare Pages static HTML guide: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/
- Cloudflare Pages Git integration: https://developers.cloudflare.com/pages/get-started/git-integration/
