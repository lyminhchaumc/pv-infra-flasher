# PV Infra Flasher

Công cụ nạp firmware cho thiết bị ESP32-C3 giám sát hạ tầng (AI Box/Camera/Hub) của Phú Vinh IOT
— chạy thẳng trên Windows, **không cần cài Arduino IDE hay PlatformIO IDE**.

Repo này **chỉ chứa công cụ phát hành (file chạy + firmware đã đóng gói)**, không chứa mã nguồn
hay dữ liệu nghiệp vụ nội bộ của công ty.

## Tải về

Vào mục **[Releases](../../releases/latest)** của repo này, tải 2 file:
- `InfraFlasher.exe` — công cụ nạp (double-click để chạy).
- `infra_watcher_v1.bin` — firmware đã gộp sẵn, nạp bằng công cụ trên.

## Cách dùng
1. Cắm board ESP32-C3 vào máy bằng cáp USB-C **có lõi dữ liệu** (không phải cáp chỉ sạc).
2. Mở `InfraFlasher.exe`.
3. Bấm "Quét lại" nếu chưa thấy cổng COM — cổng nào có chữ "Đã nhận diện..." là board thật.
4. Bấm "Chọn file..." → chọn `infra_watcher_v1.bin`.
5. Bấm "Nạp code" → chờ xong.

Mã nguồn đầy đủ (firmware .cpp, backend CRM...) nằm ở repo nội bộ riêng (không công khai).
