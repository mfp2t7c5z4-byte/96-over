# GitHub Upload Restart Checklist

- [x] Audit the current project structure and deployment configuration.
- [x] Prepare a clean GitHub-ready ZIP containing the project root files.
- [x] Verify the ZIP contains the source, package files, README, license, and deployment workflow while excluding dependencies and generated artifacts.
- [x] Provide the user with the direct download and a clean upload procedure.
- [x] Explain the correct GitHub Pages deployment setup and base-path requirements.

## Notes

The repository should contain `package.json`, `client/`, `server/`, `shared/`, `.github/`, and configuration files at the repository root, not inside an additional nested folder.

The GitHub Pages workflow must build the Vite app and deploy the generated `dist/public` output using GitHub Pages artifacts. GitHub Pages should use the GitHub Actions source after the workflow is committed.

The app uses local storage and does not require a backend service for its core functionality.

The user wants to restart the upload process after receiving a 404 from the previous Pages setup.

The current GitHub upload package must be regenerated after the final project state is verified.

The checklist will be marked complete only after the package is created and verified.

## Image Asset Repair

- [x] Trace the icon and golf background references in the source code.
- [x] Confirm the required image files are present in a deployable project directory.
- [x] Update asset paths or copy assets into the correct public location.
- [x] Rebuild and verify that the generated site contains the image assets.
- [x] Provide terminal commands for committing and pushing the repair.

## GitHub Pages Base Route Repair

- [ ] Confirm the repository name and current Vite base configuration.
- [ ] Ensure direct navigation to the repository Pages URL resolves to the app entry point.
- [ ] Preserve the asset fixes while updating the deployment package.
- [ ] Build and verify the repaired package before redeployment.
