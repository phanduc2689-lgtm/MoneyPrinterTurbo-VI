# MoneyPrinterTurbo — bản tiếng Việt

Bản này dựa trên [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) (MIT). `config.toml` đã đặt sẵn:

- Giao diện: tiếng Việt
- Ngôn ngữ kịch bản: `vi-VN`
- Giọng đọc: Hoài My (`vi-VN-HoaiMyNeural`, Edge TTS, không cần key). Giọng nam: `vi-VN-NamMinhNeural`
- Phụ đề: `BeVietnamPro-Bold.ttf` (có dấu tiếng Việt)
- Khung hình: dọc 9:16
- Mô hình viết kịch bản: Google Gemini (`gemini-3.1-pro-preview`)

## Chạy trên máy

Cần Python 3.11 trở lên và FFmpeg.

```bash
uv sync --frozen
./webui.sh
```

Rồi mở địa chỉ WebUI in ra trong terminal (mặc định cổng 8501).

## Key còn phải tự điền

Trong WebUI bấm **Cấu hình mô hình AI**:

1. Tab **Cài đặt LLM**: dán Gemini API key từ https://aistudio.google.com/app/apikey
2. Tab **Cài đặt nguồn tư liệu**: dán Pexels API key (miễn phí), hoặc chọn nguồn **Tệp cục bộ**

Không commit key lên git.
