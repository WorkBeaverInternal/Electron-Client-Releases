# Auto-Update Repository for Electron Client

This repository is dedicated to storing the necessary files for the auto-update mechanism of the Electron Client desktop application. It contains the latest release assets that the client application uses to check for updates and download only the necessary files, ensuring an efficient update process.

## Contents

- `latest.yml`: A YAML file that contains metadata about the latest release, including the version number and file URLs.
- `.blockmap`: A file that helps track changes in the application, allowing the update process to download only the modified parts of the app.
- Executable files: The necessary binaries for the latest release of the application.

## Purpose

The purpose of this repository is to serve as a storage location for the update files used by the [App Name] application. When the application detects that an update is available, it will compare the version information in the `latest.yml` file with the current installed version. If an update is available, only the necessary files (based on the `.blockmap`) will be downloaded, reducing the size of the update.

## How It Works

1. The application checks the `latest.yml` file to determine the version of the latest release.
2. If a newer version is available, the `.blockmap` file is used to identify which parts of the application need to be updated.
3. Only the updated parts are downloaded, ensuring efficient and fast updates.
4. The update is applied, and the client application is restarted.

## Adding New Releases

To add a new release to the repository:
1. Generate the new executable and blockmap files for the release.
2. Update the `latest.yml` file to reference the new version and file URLs.
3. Upload the new executable and blockmap files to this repository.
4. Tag the release in the repository to mark the new version.



