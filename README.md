# SAATHI Android Starter

This is a starter Android Studio project for the SAATHI social app. It wraps a mobile-friendly HTML prototype in an Android WebView.

## Open and build
1. Install Android Studio on a computer.
2. Extract this ZIP.
3. Android Studio > Open > select the `SAATHI_Android_Project` folder.
4. Let Gradle sync; install Android SDK Platform 35 if prompted.
5. Connect an Android phone with USB debugging enabled or use an emulator.
6. Press Run.

## Current prototype features
- Home feed, sample short-video cards, stories (expire after 24 hours in the UI), likes/comments/follow
- Profile editing, pages, notifications, share UI, demo post-data download
- Creator earnings dashboard, weekly leaderboard, demo wallet/withdrawal requests
- Demo live-stream screen and demo admin moderation panel
- Local browser storage for prototype data

## Important limitations
This is NOT a production-ready social network. The prototype stores data locally on one device. It does not yet provide real phone OTP, cloud sync, real video uploads/hosting, real live broadcasts, real advertising, actual earnings, or real money payouts. Those require a secure backend (for example Supabase), storage, an OTP provider, a live-streaming service, server-side admin roles, and a payment provider. Never treat demo wallet balances or approvals as real money.

The app's demo admin screen is not secure and must not be exposed as a real admin tool. Do not collect real UPI/bank details in this prototype.

## Build APK online with GitHub Actions (mobile-friendly, but requires GitHub repository)
A workflow is included at `.github/workflows/android.yml`. Upload the project files to a GitHub repository (not just the ZIP file), then open the repository's Actions tab. Run "Build SAATHI APK" or wait for the push build. When complete, open the workflow run, find Artifacts, and download `SAATHI-debug-APK`. This is a debug/test APK, not a Play Store release. GitHub's interface may be easier in a browser with Desktop site enabled.
