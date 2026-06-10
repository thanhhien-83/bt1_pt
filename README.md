# BÀI TẬP LỚN MÔN PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## Thông tin sinh viên

* **Họ và tên:** [Điền họ tên]
* **Mã sinh viên:** K225480106064
* **Lớp:** [Điền lớp]
* **Môn học:** Phát triển ứng dụng trên thiết bị di động - TEE0419

---

# PHẦN 1: ỨNG DỤNG MIT APP INVENTOR

## 1. Mục tiêu chương trình

Xây dựng ứng dụng trên nền tảng **MIT App Inventor** gồm 3 màn hình (Screen):

* **Screen1:** Giới thiệu thông tin bản thân và điều hướng.
* **Screen2:** Giải một bài toán đơn giản.
* **Screen3:** Hiển thị website bằng WebViewer.

Ứng dụng được phát triển bằng phương pháp kéo thả (Drag and Drop) nhằm giúp người dùng không cần viết nhiều mã lệnh nhưng vẫn xây dựng được ứng dụng Android cơ bản.

---

## 2. Thiết kế giao diện MIT App Inventor

### 2.1 Thanh công cụ trong MIT App Inventor

Trong quá trình phát triển ứng dụng, MIT App Inventor cung cấp nhiều khu vực làm việc chính:

### **Palette**

Chứa các thành phần giao diện và chức năng như:

* Button
* Label
* TextBox
* WebViewer
* Horizontal Arrangement
* Vertical Arrangement

Người dùng có thể kéo thả trực tiếp vào màn hình thiết kế.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 1 - Giao diện MIT App Inventor và Palette]`

---

### **Viewer**

Là khu vực hiển thị giao diện ứng dụng mô phỏng điện thoại Android.

Người dùng kéo thả các thành phần từ Palette sang Viewer để xây dựng giao diện.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 2 - Viewer thiết kế ứng dụng]`

---

### **Components**

Hiển thị danh sách các đối tượng đang tồn tại trong ứng dụng như:

* Button
* Label
* WebViewer
* Screen

Cho phép đổi tên hoặc quản lý thành phần.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 3 - Components]`

---

### **Properties**

Cho phép thay đổi thuộc tính của đối tượng:

Ví dụ:

* Width
* Height
* Text
* Font Size
* Background Color

Mục đích giúp thay đổi giao diện mà không cần lập trình.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 4 - Properties của Button hoặc WebViewer]`

---

## 3. Cơ chế kéo thả và Block Programming

### 3.1 Kéo thả giao diện

MIT App Inventor hoạt động theo cơ chế kéo thả.

Người dùng chỉ cần:

1. Chọn thành phần trong **Palette**
2. Kéo vào **Viewer**
3. Chỉnh thuộc tính trong **Properties**

Ví dụ:

* Kéo Button để tạo nút bấm.
* Kéo Label để hiển thị chữ.
* Kéo WebViewer để hiển thị website.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 5 - Thao tác kéo thả component]`

---

### 3.2 Block Programming là gì?

Block Programming là phương pháp lập trình trực quan bằng cách ghép các khối lệnh.

Ví dụ:

* Khi nhấn Button → thực hiện phép tính.
* Khi mở Screen → mở website.

Khối lệnh sẽ được ghép nối như các mảnh ghép logic.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 6 - Block xử lý giải toán]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 7 - Block WebViewer]`

---

### 3.3 Ưu điểm của Block so với viết Code

**Ưu điểm:**

* Dễ học
* Không cần nhớ cú pháp
* Hạn chế lỗi cú pháp
* Tốc độ phát triển nhanh

**Nhược điểm:**

* Khó mở rộng dự án lớn
* Ít linh hoạt
* Giao diện block dễ rối khi ứng dụng phức tạp

---

### 3.4 Backpack (Copy/Paste Block)

Backpack là chức năng giúp:

* Sao chép block
* Tái sử dụng block giữa các screen

Giúp tiết kiệm thời gian lập trình.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 8 - Backpack]`

---

## 4. Thiết kế ứng dụng MIT App Inventor

### 4.1 Screen1 - About

Màn hình giới thiệu thông tin sinh viên gồm:

* Họ tên
* Mã sinh viên
* Nút mở Screen2
* Nút mở Screen3

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 9 - Screen1 About]`

---

### 4.2 Screen2 - Giải toán đơn giản

Ứng dụng xây dựng chức năng giải phương trình đơn giản.

Người dùng nhập dữ liệu và nhấn nút tính để hiển thị kết quả.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 10 - Screen2 Giải toán]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 11 - Block giải toán]`

---

### 4.3 Screen3 - WebViewer

Sử dụng **WebViewer** để hiển thị website:

```text
https://k58kmt.tdh.io.vn?masv=K225480106064
```

Website được tối ưu cho giao diện điện thoại.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 12 - Screen3 WebViewer]`

---

# PHẦN 2: ỨNG DỤNG ANDROID STUDIO

## 1. Giới thiệu

Ứng dụng Android Studio được xây dựng tương đương với MIT App Inventor gồm 3 Activity:

* Activity1: About
* Activity2: Giải toán + gọi API
* Activity3: WebView

---

## 2. Tạo Project Android Studio

Tiến hành mở Android Studio và tạo project mới bằng ngôn ngữ Java.

Template sử dụng:

```text
Empty Views Activity
```

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 13 - Tạo project Android Studio]`

---

## 3. AndroidManifest.xml

### Chức năng

File `AndroidManifest.xml` dùng để:

* Khai báo Activity
* Khai báo quyền ứng dụng
* Khai báo launcher app

Ví dụ khai báo Internet:

```xml
<uses-permission
    android:name="android.permission.INTERNET"/>
```

Mục đích:

Cho phép ứng dụng kết nối API và WebView.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 14 - AndroidManifest.xml]`

---

## 4. Vòng đời ứng dụng Android

Một Activity Android có các trạng thái:

* onCreate()
* onStart()
* onResume()
* onPause()
* onStop()
* onDestroy()

Trong đó:

`onCreate()` được tự sinh sau khi tạo project vì đây là hàm khởi tạo đầu tiên của ứng dụng.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 15 - Lifecycle Android]`

---

## 5. Activity1 - About

Hiển thị:

* Thông tin cá nhân
* Nút mở Activity2
* Nút mở Activity3

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 16 - Activity1 About]`

---

## 6. Activity2 - Giải toán + API

Chức năng:

* Giải phương trình bậc 2
* Gửi dữ liệu lên API:

```text
https://k58kmt.tdh.io.vn/api
```

Dữ liệu gửi:

```json
{
 "app_by":"K225480106064",
 "input":{
   "a":1,
   "b":2,
   "c":3,
   "name":"hello tắc kè"
 },
 "output":{
   "ketluan":"vô nghiệm",
   "abc":"xyz",
   "nghiem":3.14
 }
}
```

Dữ liệu nhận về:

```json
{
 "ok":1,
 "stt":1234
}
```

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 17 - Activity2 giao diện]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 18 - Kết quả API]`

---

## 7. Activity3 - WebView

Website hiển thị:

```text
https://k58kmt.tdh.io.vn?masv=K225480106064
```

Sử dụng thành phần `WebView`.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 19 - Activity3 WebView]`

---

# KẾT LUẬN

Qua bài tập lớn, em đã tìm hiểu được:

* MIT App Inventor
* Android Studio
* WebView
* API JSON
* AndroidManifest.xml
* Activity Lifecycle
* Lập trình Java trên Android

Đồng thời giúp nâng cao kỹ năng xây dựng ứng dụng Android thực tế.
