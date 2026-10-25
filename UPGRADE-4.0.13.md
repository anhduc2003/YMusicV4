# YMusic 4.0.13 — nâng cấp (từ 4.0.12)

1. Tiếng Việt đầy đủ: values-vi thêm app_name, badge_premium, section_catalogue (trước đây thiếu 3/657 chuỗi so với bản tiếng Anh).
2. Hẹn giờ ngủ: thêm mức 120 phút (SleepTimerDialog.PresetMinutes).
3. Bộ nhớ đệm phát: thêm mức 20 GB (PlayerCacheRow).
4. Tải xuống: "Tiếp tục tất cả" (DownloadService.resumeAll) giờ xếp lại cả task PAUSED và FAILED; nút này cũng hiện khi chỉ còn task lỗi (DownloadsScreen).
5. Phiên bản: 4.0.12 -> 4.0.13, versionCode 16 -> 17 (Android, desktop, iOS).

Build Android đầy đủ cần (theo README gốc): JDK 17+, Node, CMake, Android SDK 36 + NDK 28, và checkout ffmpeg-build ngang hàng với source, rồi chạy `./gradlew :androidApp:assembleDebug` (mỗi ABI ra một APK YMusic-<version>-<abi>-release.apk).
