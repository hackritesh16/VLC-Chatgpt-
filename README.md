# VLC Neon Edition — Android

A community customization concept for VLC for Android, focused on a dark **Neon + Glass-inspired** look while keeping VLC's existing playback code untouched.

> **Project status:** Early UI theme foundation. This is not yet a complete redesign of every screen, and the APK build has not been verified. Build success depends on compatibility with the upstream VLC Android source and its current build requirements.

## ✨ Current changes

- Dark theme as the default appearance.
- Cyan and purple accent palette.
- Deep dark backgrounds and contrasting surface colors.
- Added reusable neon color resources for future UI work.
- GitHub Actions workflow to attempt a debug APK build.

## 🎨 Design direction

- **Primary accent:** Neon cyan (`#22D3EE`)
- **Secondary accent:** Neon purple (`#A855F7`)
- **Background:** Deep midnight (`#080B14`)
- **Surface:** Dark blue-grey (`#151A29`)

The current changes establish the visual theme foundation. Custom glass panels, new icons, screen-by-screen layouts, advanced animations, and in-app theme/font customization still need to be implemented and tested separately.

## 🧰 Build an APK with GitHub Actions

1. Create a GitHub repository for your copy of this project.
2. Upload the contents of this ZIP to the repository. Make sure `README.md` and `.github/workflows/build-apk.yml` are included.
3. Push the files to the `main` or `master` branch.
4. Open the repository's **Actions** tab.
5. Select **Build VLC Neon APK** and choose **Run workflow** if the workflow has not already started.
6. When the run finishes, open the workflow run and download the **VLC-Neon-debug-APK** artifact.

The workflow fetches the upstream VLC Android repository and its submodules, then overlays this project's files because the supplied source archive does not contain every upstream build component.

## ⚠️ Important notes

- This is an unofficial customization project and is not an official VideoLAN release.
- The workflow is a build attempt, not a guarantee that the current source will compile. If it fails, open the failed GitHub Actions run and inspect the first actual Gradle/build error.
- A debug APK is for testing. Do not assume it is production-ready or suitable for publishing.
- VLC and its upstream components retain their respective licenses. Review the upstream repository and license notices before redistributing builds or source.

## 📁 Main files

- `application/resources/src/main/res/values/colors.xml` — reusable neon color resources.
- `application/vlc-android/res/values/styles.xml` — theme and appearance colors.
- `.github/workflows/build-apk.yml` — GitHub Actions debug-build workflow.
- `NEON-UI-CHANGES.md` — summary of the initial theme changes and source limitations.

## 🙌 Credits

Based on the VLC for Android source code maintained by the VideoLAN community. This project is an independent UI customization effort.
