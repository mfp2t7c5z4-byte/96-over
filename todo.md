# GitHub Upload Restart Checklist

- [ ] Audit the current project structure and deployment configuration.
- [ ] Prepare a clean GitHub-ready ZIP containing the project root files.
- [ ] Verify the ZIP contains the source, package files, README, license, and deployment workflow while excluding dependencies and generated artifacts.
- [ ] Provide the user with the direct download and a clean upload procedure.
- [ ] Explain the correct GitHub Pages deployment setup and base-path requirements.

## Notes

The repository should contain `package.json`, `client/`, `server/`, `shared/`, `.github/`, and configuration files at the repository root, not inside an additional nested folder.

The GitHub Pages workflow must build the Vite app and deploy the generated `dist/public` output using GitHub Pages artifacts. GitHub Pages should use the GitHub Actions source after the workflow is committed.

The app uses local storage and does not require a backend service for its core functionality.

The user wants to restart the upload process after receiving a 404 from the previous Pages setup.

The current GitHub upload package must be regenerated after the final project state is verified.

The checklist will be marked complete only after the package is created and verified.
