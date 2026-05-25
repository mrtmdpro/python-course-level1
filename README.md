# Khoá học Python cho học sinh THPT

# Python Course for Vietnamese High-School Beginners

Một khoá học **Python từ con số 0** dành cho học sinh THPT (15-18 tuổi),
gồm **16 buổi × 90 phút**, học trong **2 tháng** (2 buổi/tuần).
Sau khoá học, người học hiểu được các khái niệm lập trình cốt lõi và
xây dựng được một dự án Python nhỏ của riêng mình.

_A 16-session, 90-minute, 8-week Python course for Vietnamese high-school
beginners. Bilingual notebooks (Vietnamese explanations + English technical
terms). After the course, learners understand core programming concepts and
can build their own small Python project._

---

## 1. Đối tượng & mục tiêu / Audience & outcomes

- **Đối tượng:** học sinh THPT (15-18 tuổi), chưa từng lập trình.
- **Yêu cầu trước:** không — chỉ cần biết dùng máy tính cơ bản và có tài khoản Google
  (cho Google Colab).
- **Sau khoá học, người học có thể:**
  - Đọc, viết, gỡ lỗi (debug) các chương trình Python cơ bản.
  - Sử dụng biến, kiểu dữ liệu, vòng lặp, điều kiện, hàm, list/dict, file I/O.
  - Áp dụng pandas/matplotlib hoặc turtle để xây dự án nhỏ.
  - Hoàn thành 1 dự án **capstone** đầu đời và trình bày được.

---

## 2. Cách cài đặt / Setup

Khoá học hỗ trợ **2 môi trường**: Google Colab (khuyến khích cho buổi đầu) và
VS Code + Python + Jupyter extension (cho ai muốn cài máy local).

### Cách A — Google Colab (browser, không cần cài)

1. Truy cập <https://colab.research.google.com>.
2. Đăng nhập bằng tài khoản Google.
3. Tải notebook về máy (chuột phải → `Save as`) hoặc clone repo này về Google Drive.
4. Trong Colab: `File` → `Upload notebook` → chọn file `.ipynb` của buổi học.
5. Bấm `Shift + Enter` để chạy từng cell.

> **Tip:** trong Colab, dữ liệu trong `assets/data/` chưa có sẵn.
> Tải các file CSV về Drive hoặc upload thủ công vào session.

### Cách B — VS Code + Python + Jupyter (local)

1. Cài Python 3.10 hoặc 3.11 từ <https://www.python.org>.
2. Cài VS Code từ <https://code.visualstudio.com>.
3. Trong VS Code, mở tab **Extensions** và cài 2 extension:
   - `Python` (Microsoft)
   - `Jupyter` (Microsoft)
4. Clone hoặc tải repo này về máy.
5. Mở terminal trong thư mục repo và chạy:
   ```bash
   pip install -r requirements.txt
   ```
6. Mở `sessions/Session_01_Welcome_and_Setup.ipynb` — VS Code tự nhận diện kernel.

---

## 3. Cấu trúc kho / Repository layout

```
.
├── README.md                       # file này
├── requirements.txt                # pip dependencies cho local install
├── sessions/                       # 16 notebook cho học sinh
│   ├── Session_01_Welcome_and_Setup.ipynb
│   ├── ...
│   └── Session_16_Demo_Day_and_Whats_Next.ipynb
├── appendix/                       # tài liệu tham khảo
│   └── Appendix_A_FAQ_Data_Structures_and_Algorithms.ipynb
└── assets/
    ├── data/                       # CSV mẫu cho capstone Track B
    │   ├── weather_hanoi.csv
    │   └── school_grades.csv
    └── images/                     # (rỗng, dành cho diagrams sau này)
```

---

## 4. Lịch học 16 buổi / 16-session schedule

| # | Buổi | Title | Trọng tâm / Focus |
|---|------|-------|-------------------|
| 1 | Chào mừng & Cài đặt | Welcome & Setup | Colab/VS Code, `print()`, comments, đọc lỗi |
| 2 | Biến & Kiểu dữ liệu | Variables & Types | `int`, `float`, `str`, `bool`, type conversion |
| 3 | Chuỗi & Nhập | Strings & Input | `input()`, indexing, slicing, methods, f-strings |
| 4 | Câu lệnh điều kiện | Conditionals | `if/elif/else`, comparisons, `and/or/not` |
| 5 | Vòng lặp while | While Loops | `while`, `break`, `continue`, input validation |
| 6 | for & range() | For Loops & range() | accumulator pattern, nested loops, FizzBuzz |
| 7 | List | Lists | indexing, slicing, methods, iteration |
| 8 | Tuple, Set, Dict | Tuples, Sets, Dicts | khi nào dùng cái nào, đếm tần suất |
| 9 | Dữ liệu lồng & Comprehension | Nested Data & Comprehensions | 2D, list of dicts, list comprehension |
| 10 | Hàm | Functions | `def`, `return`, scope, decomposition |
| 11 | Module & Thư viện chuẩn | Modules & Stdlib | `math`, `random`, `datetime`, viết module riêng |
| 12 | File & CSV | Files & CSV | `with open`, `csv`, intro pandas |
| 13 | Lỗi & Debug | Errors & Debugging | `try/except`, traceback, print debugging |
| 14 | Capstone — Khởi động | Capstone — Kickoff | chọn 1/3 tracks, lên plan, scaffold |
| 15 | Capstone — Build & Iterate | Capstone — Build & Iterate | code review, edge cases, refactor |
| 16 | Demo Day & Sau khoá | Demo Day & What's Next | demo 3 phút, peer review, hành trình tiếp |

Mỗi buổi 90 phút theo chuẩn:

- **0-10 min** Khởi động & ôn bài (warm-up + recap)
- **10-40 min** Lý thuyết + live coding
- **40-70 min** Bài tập tại lớp (in-class exercises)
- **70-85 min** Thử thách của buổi (challenge of the day)
- **85-90 min** Tổng kết, từ vựng (Vi↔En), giao bài về nhà

---

## 5. Capstone — 3 tracks

Sau 13 buổi nền tảng, ở Buổi 14 học sinh chọn **1 trong 3 tracks** dự án và
hoàn thành trong 3 buổi cuối. Demo Day diễn ra ở Buổi 16.

| Track | Tóm tắt | Modules chính |
|-------|---------|---------------|
| **A — Quiz / Game văn bản** | 10 câu hỏi, trộn ngẫu nhiên, tính điểm, lưu high-score CSV | `random`, `csv`, `datetime` |
| **B — Phân tích dữ liệu** | Đọc CSV thật (thời tiết / điểm), thống kê, vẽ biểu đồ | `pandas`, `matplotlib` |
| **C — Visual với matplotlib** | Tạo mosaic / fractal generative art (chạy được trên Colab) | `matplotlib`, `random`, `math` |

Yêu cầu cuối (Buổi 16):

- Code chạy không lỗi với 3 kịch bản test (happy / failure / edge).
- README markdown ở đầu notebook (mục đích + cách chạy).
- Tối thiểu 5 hàm tự viết, mỗi hàm có docstring.
- Có ít nhất 1 chỗ xử lý lỗi (`try/except`).
- Có hiển thị / biểu đồ / giao diện đẹp.

---

## 6. Cách dùng notebook / How to use the notebooks

1. Mở notebook tương ứng buổi học (`sessions/Session_XX_*.ipynb`).
2. Đọc từ trên xuống dưới — không bỏ qua các ô markdown.
3. Mỗi ô code có thể chạy bằng `Shift + Enter`.
4. Phần **Bài tập tại lớp** và **Bài tập về nhà** có ô code trống `# TODO`
   để bạn viết bài làm.
5. Khi gặp lỗi: đọc dòng cuối của thông báo lỗi trước.
6. Lưu file thường xuyên (Colab tự lưu vào Drive, VS Code dùng `Ctrl+S`).

### Phụ lục / Appendix

Trong thư mục `appendix/` có **sổ tay tra cứu** cho các câu hỏi thường gặp về
**cấu trúc dữ liệu và giải thuật** (đảo chuỗi, palindrome, lambda, sorting,
binary search, two pointers, sliding window, đệ quy, ...). Mở khi gặp khó
hoặc khi muốn học thêm — không cần đọc một lèo, dùng như từ điển.

_The `appendix/` folder is a quick-reference cheat sheet for common Python
questions on data structures and algorithms — open it when stuck or curious.
Skim by topic, not cover-to-cover._

---

## 7. Tài nguyên thêm / Further resources

- **Python docs (chính thức):** <https://docs.python.org/3/tutorial/>
- **Real Python:** <https://realpython.com> — bài viết chất lượng cao.
- **Automate the Boring Stuff with Python** (miễn phí online): <https://automatetheboringstuff.com>
- **Kaggle Learn:** <https://www.kaggle.com/learn> — Python, pandas, ML miễn phí.
- **Codewars / LeetCode:** luyện kata sau khoá học.
- **Cộng đồng VN:** Daynhauhoc, Facebook Group Lập trình Python Việt Nam.

---

## 8. Quy tắc trong lớp / Classroom rules

- **Chạy code thường xuyên** — đừng đợi viết hết rồi mới chạy.
- **Đoán trước khi chạy** — sai thì học được nhiều hơn đoán đúng.
- **Hỏi khi bí 5 phút** — đừng kẹt 30 phút một mình.
- **Khen trước, góp ý sau** khi review code của bạn cùng lớp.
- **Hoàn thành thay vì hoàn hảo** — code chạy được luôn tốt hơn code dở dang.

---

Chúc các bạn **học vui và code đều** 🐍
_(Have fun and keep coding 🐍)_
