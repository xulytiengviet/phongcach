# PHONGCÁCH — 30 điểm bắt đầu khác biệt

Thư viện tiếng Việt gồm **30 mẫu HTML + CSS độc lập**, chia đúng 3 nhóm × 10. Chọn phong cách, xem trước, sao chép mã và prompt để giao AI phát triển tiếp.

**Demo dự kiến khi GitHub Pages triển khai thành công:** https://xulytiengviet.github.io/phongcach/

## Sử dụng

Mở `index.html` trực tiếp hoặc chạy `python -m http.server 8000` rồi truy cập http://localhost:8000. Không cần npm, framework, font ngoài, CDN hoặc backend.

- Lọc theo nhóm; tìm kiếm tiếng Việt có hoặc không dấu.
- Xem trước desktop/mobile 375px; xem riêng HTML và CSS.
- Copy HTML, CSS, prompt hoặc toàn bộ mã + prompt; thêm yêu cầu dự án trước khi copy.
- Tải từng mẫu `.html`; mở mẫu độc lập từ `templates/`.
- Đường dẫn `index.html#royal` mở trực tiếp mẫu Royal Burgundy.
- Hỗ trợ Escape, bàn phím, focus, reduced motion và thông báo clipboard.

## Danh mục

| Dev / DevOS / Hacker | Độc lạ & Thử nghiệm | Neon / Cổ điển / Hoàng gia |
|---|---|---|
| Terminal xanh | Neo-brutal Playground | Neon Tokyo |
| DevOS Desktop | Swiss Editorial | Synthwave 84 |
| Midnight Engineer | Bauhaus Lab | Art Deco |
| Code Editor | Paper Collage | Royal Burgundy |
| API Blueprint | Kinetic Type | Victorian Gazette |
| README Studio | Organic Studio | Luxury Noir |
| Cyber Ops | Bento Workshop | Cobalt Neon |
| CRT Phosphor | Wireframe Notes | Retro Diner |
| CLI Manual | Isometric Blocks | Celestial Observatory |
| Git Workflow | Museum Label | Classic Library |

## Cấu trúc và chỉnh sửa

- `index.html`: gallery, giao diện và thao tác copy/tải.
- `data.js`: catalog nhúng, hoạt động cả với `file://`.
- `catalog.json`: dữ liệu có cấu trúc cho công cụ khác.
- `templates/*.html`: 30 file độc lập, CSS nằm trong `<style>`.
- `build_templates.py`: nguồn dữ liệu, HTML và CSS từng phong cách. Chạy `python build_templates.py` để tái tạo data.js, catalog.json và templates. Không ghi đè index.html.
- `.github/workflows/pages.yml`: triển khai GitHub Pages khi push `main`.

Các template dùng CSS variables `--bg`, `--fg`, `--accent`, `--font`. Nội dung, email example.com và trạng thái vận hành đều là minh họa; cần thay và kiểm tra trước khi dùng thật. Các mẫu terminal/editor/desktop là giao diện HTML/CSS, không phải terminal hay hệ điều hành thực. Prompt là chỉ dẫn để copy sang AI, không tự gọi API.

## Nguồn cảm hứng

Thiết kế tự viết từ mô tả của người dùng và đoạn HTML Neo-brutalism đính kèm; không sao chép mã từ các thương hiệu, không tuyên bố liên kết với họ. Các liên kết sau để tham khảo định hướng thị giác, không phải dependency hay xác nhận giao diện hiện tại:

- [Gitingest](https://gitingest.com/): viền rõ, bóng cứng và màu pastel.
- [LiveTerm](https://github.com/Cveinnt/LiveTerm): ý tưởng portfolio terminal.
- [Warp](https://www.warp.dev/), [PlanetScale](https://planetscale.com/), [Tinybird](https://www.tinybird.co/): văn hóa giao diện công cụ developer.
- Các trào lưu Bauhaus, Swiss, Art Deco, retro computing và typography editorial.

Không phân phối template thương mại của Framer. Mã trong repo được cung cấp theo MIT; thương hiệu được nhắc tới thuộc chủ sở hữu tương ứng.

## Triển khai

Workflow thử khởi tạo GitHub Pages qua `configure-pages`. Nếu tài khoản không cho Actions bật Pages, chọn **Settings → Pages → Source → GitHub Actions**, rồi chạy lại workflow. URL demo chỉ hoạt động sau lần deploy thành công.

Long Ngo · MIT
