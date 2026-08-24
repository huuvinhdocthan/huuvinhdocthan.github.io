# Zinh Doan ~ AVL ~ Sound and Event Tool

Bộ công cụ web tĩnh (chạy offline, không cần server/backend) phục vụ công việc kỹ thuật Âm thanh - Ánh sáng - Sự kiện. Thực hiện bởi **Zinh Doan — Freelancer AVL**.

- Gmail: Huuvinhit98@gmail.com

## Cấu trúc

| File | Mô tả | Trạng thái |
|---|---|---|
| `index.html` | Trang tổng — danh sách các công cụ, bấm vào để mở | ✅ |
| `mapping_led.html` | LED Slice Mapper — sắp xếp slice, tự tính Composition cho Resolume, xoay/cắt hình, xuất PNG test pattern | ✅ |
| `soundboard.html` | Soundboard sự kiện — kéo thả nhạc/hiệu ứng, phím tắt, fade in/out, playlist | ✅ |
| `countdown.html` | Đếm ngược sự kiện — đồng hồ đếm ngược cho MC/diễn giả khi thuyết trình PPT, cảnh báo vàng/đỏ, tự đếm vượt giờ, chế độ trình chiếu toàn màn hình, tùy chỉnh màu nền/số/chữ/vòng tròn | ✅ |
| `dmx_calculator.html` | DMX Calculator — tính địa chỉ DMX theo số đèn/số kênh, tự chia Universe, cảnh báo trùng địa chỉ, bản đồ kênh trực quan, xuất patch list .txt | ✅ |
| `power_calculator.html` | Power Calculator — tính tổng công suất & dòng điện (Ampere) theo pha/điện áp, cân tải L1/L2/L3, gợi ý CB & tiết diện dây, xuất báo cáo .txt | ✅ |
| `pad_play_music_2.html` | Pad Play Music 2 — Music Player nhạc nền tự chuyển bài + DJ Sound Pad 15 nút hiệu ứng/nhạc dẫn MC, phím tắt bàn phím, thêm hàng loạt Pad cùng lúc | ✅ |
| `run_of_show.html` | Run of Show — bảng kịch bản chương trình có đếm ngược | ⏳ sắp làm |

## Chạy thử trên máy

Không cần cài gì cả — mở trực tiếp `index.html` bằng trình duyệt (double-click là chạy).

## Giao diện Sáng / Tối

Mọi trang đều có nút 🌙/☀️ ở góc trên bên phải để đổi giao diện. Mặc định là **giao diện sáng**, và tự chuyển sang tối nếu máy đang để hệ điều hành ở chế độ tối — cho tới khi bạn tự bấm chọn, lúc đó lựa chọn sẽ được nhớ chung cho cả site (dùng `localStorage`, chỉ cần chọn 1 lần, áp dụng luôn khi mở sang trang khác).

## Website sống

Repo này là repo **user site** (`huuvinhdocthan.github.io`) nên GitHub Pages tự chạy ở gốc domain — chỉ cần `git push` là trang cập nhật tại `https://huuvinhdocthan.github.io/` (không cần bật lại Settings → Pages, vì loại repo `username.github.io` đã tự bật sẵn).

## Thêm tool mới

1. Thêm file `.html` mới vào repo (cùng cấp với `mapping_led.html`).
2. Mở `index.html`:
   - Nếu tool đang nằm ở nhóm **"Sắp ra mắt"**: đổi `<div class="tool soon">` thành `<a class="tool" href="ten-file.html">`, đổi khối `<div class="badge">Sắp ra mắt</div>` thành `<div class="open">Mở công cụ →</div>`, rồi cắt cả khối chuyển lên nhóm **"Đang dùng được"** phía trên.
   - Nếu là tool hoàn toàn mới: copy khối `<a class="tool">...</a>` có sẵn, sửa `href`, icon, tiêu đề, mô tả, tag cho phù hợp.
3. Commit & push — nếu đã bật GitHub Pages ở bước trên thì trang tổng tự cập nhật, không cần làm gì thêm.

## Cập nhật & đẩy lên GitHub

```bash
git add .
git commit -m "Mô tả thay đổi"
git push
```

## Bản quyền

© 2026 Zinh Doan. Bảo lưu mọi quyền — xem chi tiết ở file [`LICENSE`](./LICENSE). Đây không phải phần mềm mã nguồn mở; nghiêm cấm sao chép, phân phối lại hoặc sử dụng lại mã nguồn khi chưa có sự đồng ý bằng văn bản.
