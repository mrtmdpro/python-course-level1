# Sample datasets / Bộ dữ liệu mẫu

Hai bộ dữ liệu này dùng cho **Capstone Track B — Data analysis**.

| File | Cột | Mô tả |
|------|-----|-------|
| `weather_hanoi.csv` | `date, temp_c, humidity_pct, rain_mm` | 30 ngày thời tiết Hà Nội (mock) — tháng 5/2026 |
| `school_grades.csv` | `ten, lop, toan, van, anh, ly, hoa` | 30 học sinh, 5 môn — điểm thang 10 |

Cả hai dữ liệu đều **giả lập** (random với seed cố định để mỗi lần dựng lại đều giống nhau).
Có thể tạo lại bất kỳ lúc nào bằng `python tools/make_assets.py`.

## Cách đọc nhanh

```python
import pandas as pd
df = pd.read_csv("assets/data/weather_hanoi.csv")
print(df.head())
```

Trên Colab khi chạy notebook trong `sessions/`, đường dẫn tương đối là `'../assets/data/weather_hanoi.csv'`.
