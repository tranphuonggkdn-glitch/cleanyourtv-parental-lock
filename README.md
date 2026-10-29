# CleanYourTV Parental Time Lock — R15 Pilot

> **Community derivative / pre-release.** This package is independent of, and not endorsed by, the original [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) project.

Bộ cài thử nghiệm **CleanYourTV R15** cho **Android TV / Google TV (Android 11 trở lên)**. Tính năng dự kiến: launcher đơn giản; giới hạn thời gian theo ngày; khung giờ được xem; PIN phụ huynh; phút thưởng; đồng hồ đã dùng / còn lại; giữ màn hình khóa khi bấm Home/Back trên TCL G07 đã thử.

**Chưa phải ứng dụng khóa trẻ em đạt mức bảo vệ hệ thống.** Firmware TV khác nhau có thể cho phép chuyển Home hoặc thoát khỏi ứng dụng; chưa nghiệm thu R15 khóa liên tục quá 10 phút trên TCL và chưa nghiệm thu trên các hãng TV khác. Chỉ thử trên TV do bạn sở hữu, có người lớn giám sát, không coi là biện pháp an toàn tuyệt đối.

## Cài đặt

1. Chuẩn bị máy Windows có **Android SDK Platform Tools (`adb`)** và **Build-Tools 34 (`apksigner`)**. Bật ADB debugging / Wireless debugging trên TV Android mới và xác nhận kết nối.
2. Trong mục **Releases**, tải **`INSTALL_OTHER_ANDROID_TV_ONECLICK.bat`** (bản độc lập đã nhúng APK), hoặc tải ZIP gồm đầy đủ hướng dẫn và APK.
3. Chạy `.bat`, nhập serial hoặc IP:port ADB của TV mới, kiểm tra tên thiết bị rồi gõ **`INSTALL`** để xác nhận.
4. Installer **chỉ cho cài mới** và dừng nếu TV đã có `com.gathin.tvhome`. Installer **không** tự thay launcher mặc định, không bật Accessibility, không reset TV, không tắt ứng dụng hãng, không sửa PIN.
5. Mở CleanYourTV trên TV từ danh sách ứng dụng, thiết lập PIN và thời gian; kiểm tra bằng remote: hiển thị phút còn lại, Home/Back trong lúc khóa, mở khóa bằng PIN, tắt/bật TV và khóa liên tục trên 10 phút.

**Không dùng APK này cho LG webOS hoặc Samsung Tizen.** Các hệ điều hành đó cần ứng dụng native tương ứng hoặc dùng thiết bị Android TV nối qua HDMI (chỉ kiểm soát nội dung trên thiết bị Android).

## Tính toàn vẹn

- Package: `com.gathin.tvhome`
- R15 APK SHA256: `e4b64d52ad25b88ac50d2d2594ace074391cf7ef00790dbaf66dc1e0125efa03`
- Certificate SHA256: `e2e97a5ce9b617a1f053e3f2c25ffb736609e516fa039dba589385e2368ab742`
- **Đây là APK thử nghiệm, chưa phải bản phát hành production.** Không dùng chứng chỉ thử nghiệm làm căn cứ duy nhất để tin cậy mọi bản APK khác.

## Ghi công và giấy phép

Launcher dựa trên mã nguồn CleanYourTV của [Gathin23](https://github.com/Gathin23/cleanyourtv), giấy phép **MIT**, ghi công Gathin (2026). Phông **Outfit** thuộc Outfit Project Authors, theo **SIL Open Font License 1.1**. Xem `LICENSE` và `FONT-LICENSE-OFL.txt`. Đây là bản phát triển độc lập bổ sung tính năng parental lock, không phải phát hành chính thức của Gathin23.

## Lưu ý về source

Đây là **gói phân phối APK và trình cài**, không phải toàn bộ source code của nhánh R15. Source của dự án nền tảng có tại liên kết phía trên. Không cung cấp bản debug keystore hay tài liệu evidence riêng tư.
