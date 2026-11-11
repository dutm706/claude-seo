# Claude SEO – Bản Bống Media

Bộ công cụ SEO chạy trong **Claude Code**: 26 skills và 19 agent chuyên trách, audit toàn bộ website trong 10–15 phút và trả về kế hoạch hành động ưu tiên.

Bản này được fork từ [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo) (giấy phép MIT) và tùy biến cho Bống Media:

- Báo cáo, kế hoạch và dàn ý bài viết bằng **tiếng Việt**
- Kiến thức thị trường Việt Nam: từ khoá có dấu/không dấu, slug không dấu, Zalo/Facebook, địa chỉ theo sắp xếp hành chính từ 1/7/2025, dấu Bộ Công Thương
- Hồ sơ sẵn các website: bongmedia.vn, xshdsolar.vn

## Cài đặt

Cần Claude Code (tab **Code** trong app Claude trên máy tính, hoặc lệnh `claude` trong Terminal). Gõ lần lượt:

```
/plugin marketplace add dutm706/claude-seo
/plugin install claude-seo@bongmedia-claude-seo
/seo setup
```

`/seo setup` tạo môi trường Python riêng và trình duyệt ẩn để quét website, không ảnh hưởng phần còn lại của máy. Kiểm tra bất cứ lúc nào bằng `/seo doctor`.

## Lệnh hay dùng

| Lệnh | Việc làm |
|------|----------|
| `/seo audit https://bongmedia.vn` | Audit toàn site, chấm điểm 0–100, kế hoạch ưu tiên |
| `/seo page <url>` | Phân tích sâu một trang |
| `/seo technical <url>` | Kỹ thuật: index, tốc độ, Core Web Vitals, bảo mật |
| `/seo content <url>` | Chất lượng nội dung, E-E-A-T |
| `/seo content-brief <chủ đề>` | Dàn ý bài viết chuẩn SEO, từ khoá, liên kết nội bộ |
| `/seo cluster <từ khoá>` | Gom cụm từ khoá theo kết quả Google |
| `/seo schema <url>` | Kiểm tra và tạo Schema (JSON-LD) |
| `/seo geo <url>` | Khả năng được ChatGPT, Gemini, AI Overviews trích dẫn |
| `/seo local <url>` | SEO địa phương, Google Business Profile, NAP |
| `/seo images <url>` | Tối ưu hình ảnh |
| `/seo drift baseline <url>` | Lưu mốc để theo dõi thay đổi sau này |
| `/seo google report` | Xuất báo cáo PDF |

Có thể gọi theo tên thương hiệu, ví dụ: `/seo audit XSHD`.

## Thêm website

Mở `skills/seo/references/bongmedia-sites.md`, thêm một dòng vào bảng, rồi commit lên repo này. Sau đó cập nhật plugin trong Claude Code:

```
/plugin marketplace update bongmedia-claude-seo
```

## Nhận bản cập nhật từ tác giả gốc

Trên GitHub, mở repo `dutm706/claude-seo` → bấm **Sync fork** → **Update branch**. Nếu GitHub báo xung đột, giữ phần tùy biến Bống Media (các file trong danh sách bên dưới).

Các file đã tùy biến:
- `.claude-plugin/marketplace.json` (tên marketplace)
- `skills/seo/SKILL.md` (cấu hình tiếng Việt, footer)
- `skills/seo/references/vietnam-market.md`, `skills/seo/references/bongmedia-sites.md`
- Một dòng chỉ dẫn tiếng Việt ở đầu mỗi `skills/seo-*/SKILL.md` và `agents/seo-*.md`
- `README.vi.md`

Tài liệu đầy đủ (tiếng Anh): [README.md](README.md).
