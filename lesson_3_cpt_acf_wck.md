# Lesson 3: Sử dụng Custom Post Type và Custom Fields trong WordPress

Trong WordPress, ngoài bài viết (Post) và trang (Page) mặc định, chúng ta có thể tạo các loại nội dung chuyên biệt để quản lý dữ liệu hiệu quả hơn.

---

## 1. Custom Post Type (CPT)

- **Custom Post Type (CPT)** là loại bài viết tùy chỉnh, cho phép quản lý nội dung chuyên biệt ngoài Post/Page mặc định.
- Lợi ích:
  - Tách biệt các loại nội dung khác nhau (ví dụ game, nhân vật, sự kiện)
  - Dễ dàng quản lý, hiển thị và tìm kiếm trên website
- Ví dụ cho blog game:
  | CPT | Mục đích |
  |-----|----------|
  | Game | Lưu thông tin game (tên, thể loại, nền tảng, điểm, cover image) |
  | Character | Lưu thông tin nhân vật game (tên, vai trò, sức mạnh, avatar) |
  | Review | Lưu đánh giá game (score, pros, cons, cover image, release date) |

---

## 2. Custom Fields

- **Custom Fields** là các dữ liệu bổ sung gắn vào mỗi bài viết hoặc CPT, giúp lưu thông tin chi tiết hơn so với title/content mặc định.
- Ví dụ cho CPT `Game`:
  - score: điểm đánh giá game
  - genre: thể loại
  - platform: nền tảng (PC, Mobile, Console)
  - release_date: ngày phát hành
  - cover_image: ảnh minh họa
- **Advanced Custom Fields (ACF)** hoặc **WCK – Custom Fields and Custom Post Types Creator** giúp tạo field trực quan, dễ quản lý mà không cần code nhiều.

---

## 3. Plugin WCK – Custom Fields and Custom Post Types Creator

- WCK cho phép:
  1. **Tạo Custom Post Type** mà không cần lập trình
  2. **Tạo Custom Meta Boxes / Custom Fields** dễ dàng
  3. **Thiết lập Repeater, Sortable, Conditional Fields** để quản lý dữ liệu linh hoạt
  4. Gắn meta box vào CPT, Page hoặc Post ID cụ thể
- Cách sử dụng cơ bản:
  1. Cài và kích hoạt plugin WCK
  2. Tạo CPT mới (ví dụ: `game`)
     - Điền Post Type, Description, Singular Label, Plural Label
     - Chọn có Archive hay không, hỗ trợ title, editor, thumbnail...
  3. Tạo **Custom Meta Box**:
     - Chọn Group Name, Post Type gắn vào
     - Thêm field: game_name (text), score (number), pros (textarea), cons (textarea), cover_image (upload)
     - Chỉ định Required, Default Value, Min/Max, Step Value (cho số)
  4. Khi tạo bài viết trong CPT `game`, meta box sẽ xuất hiện, nhập dữ liệu cho từng game riêng biệt.
- **Lưu ý:** 1 meta box + field có thể áp dụng cho tất cả bài viết CPT, không cần tạo lại cho từng bài.

---

## 4. Kết luận

- **Custom Post Type** giúp tách loại nội dung chuyên biệt, dễ quản lý và hiển thị.
- **Custom Fields** lưu trữ dữ liệu chi tiết cho từng bài viết.
- **WCK** giúp tạo CPT và Custom Fields trực quan, dễ sử dụng, phù hợp với blog game hoặc bất kỳ nội dung chuyên biệt nào.
- Khi kết hợp CPT + Custom Fields, bạn có thể quản lý nội dung blog một cách chuyên nghiệp và mở rộng dễ dàng.
