# EXP Block Ads

Kênh APK thử nghiệm công khai cho EXP Block Ads (Android 8 trở lên). Repo này chỉ chứa thông tin phát hành; mã nguồn được quản lý riêng.

## Cài đặt

Tải `exp-block-ads.apk` tại [Releases mới nhất](https://github.com/manhninh94/exp-block-ads-releases/releases/latest). Cài đè bản đang dùng để giữ cấu hình. Bản trước 0.2.0 cần cài thủ công một lần lên 0.2.0 để có updater.

Trong app, mục **Cập nhật ứng dụng** cho phép kiểm tra phiên bản mới. Mặc định kiểm tra khoảng mỗi ngày; có thể tắt. App thông báo bản mới nếu đã được cấp quyền thông báo. Chỉ tải khi bạn chọn cập nhật và mở trình cài đặt Android sau khi kiểm tra file. Android yêu cầu quyền cài từ nguồn này và xác nhận cài đặt; app không tự cài im lặng.

## Lọc quảng cáo

VPN cục bộ lọc DNS ngay trên điện thoại; web/game không đi qua máy chủ VPN trung gian, giữ IP mạng hiện tại. Cập nhật danh sách lọc để tải bộ tên miền đầy đủ. Không dùng cùng VPN khác. Chỉ hỗ trợ DNS hệ thống IPv4/UDP trong bản thử, chưa hỗ trợ DNS TCP. DNS riêng tư/DoH của app và quảng cáo dùng chung tên miền nội dung có thể bỏ qua bộ lọc. Không cam kết chặn tất cả quảng cáo.

## Dữ liệu và cập nhật

App không có tài khoản và không tích hợp analytics. Tên miền được xử lý trong bộ nhớ để lọc; app không lưu lịch sử tên miền. Cấu hình, danh sách lọc, metadata cập nhật và APK tải về được lưu trong vùng riêng của app. Bộ đếm DNS được giữ trong phiên chạy. Gỡ app sẽ xóa dữ liệu cục bộ.

Truy vấn DNS được chuyển tiếp qua HTTPS tới **Control D Ads & Tracking** hoặc **AdGuard DNS** nếu cần. Các nhà cung cấp đó có thể thấy IP và tên miền được hỏi. Danh sách lọc tải từ GitHub (HaGeZi). Kiểm tra/tải cập nhật app cũng kết nối GitHub; GitHub có thể ghi nhận IP và thông tin kết nối theo chính sách của họ. Không có token GitHub trong APK.

- [Control D privacy](https://controld.com/privacy)
- [AdGuard DNS privacy](https://adguard-dns.io/en/privacy.html)
- [GitHub privacy](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)
- [HaGeZi nguồn/giấy phép danh sách](https://github.com/hagezi/dns-blocklists)

APK được đối chiếu SHA-256, package, phiên bản và chứng thư ký của app đang cài. Android installer là bên xác minh chữ ký và cài đặt cuối cùng. Đây là kênh thử nghiệm, chưa đảm bảo tương thích mọi ROM. Luồng cài updater cần tiếp tục được xác nhận trên thiết bị thật.

Báo lỗi qua [Issues](https://github.com/manhninh94/exp-block-ads-releases/issues), kèm phiên bản app và Android.
