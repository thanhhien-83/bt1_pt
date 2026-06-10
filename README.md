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

`onCreate()` được Android Studio tự động sinh sau khi tạo project vì đây là hàm đầu tiên chạy khi Activity được khởi tạo.

Hàm này có nhiệm vụ:

* Khởi tạo giao diện bằng `setContentView()`
* Ánh xạ View với `findViewById()`
* Xử lý logic ban đầu của chương trình.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 15 - Lifecycle Android]`

---

# PROJECT 1 - APP1 (FOOD GUIDE APP)

## 5. Giới thiệu ứng dụng App1

Ứng dụng App1 được xây dựng bằng Android Studio sử dụng cơ chế **Assets** để lưu dữ liệu chuẩn bị trước dưới dạng JSON.

Mục tiêu ứng dụng:

* Hiển thị món ăn vùng miền Việt Nam.
* Tìm kiếm món ăn theo tên.
* Lọc món ăn theo tỉnh thành.
* Hoạt động offline nhờ dữ liệu được lưu sẵn trong Assets.

Dữ liệu được lưu trong file:

```text
foods.json
```

---

## 6. Thư mục Assets

Android Studio hỗ trợ thư mục đặc biệt:

```text
assets
```

Các file trong thư mục này sẽ được đóng gói đi cùng ứng dụng khi build APK.

Nhờ đó ứng dụng vẫn hoạt động được kể cả khi không có Internet.

Ví dụ:

```java
InputStream is =
        getAssets().open("foods.json");
```

Lệnh trên dùng để đọc file dữ liệu JSON từ thư mục Assets.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 16 - Thư mục assets và foods.json]`

---

## 7. Giao diện ứng dụng App1

Giao diện gồm:

* Thanh tìm kiếm món ăn.
* Bộ lọc tỉnh thành.
* Danh sách món ăn.
* Khu vực hiển thị thông tin chi tiết.

Các thành phần giao diện được mô tả trong file XML tại:

```text
res/layout/activity_main.xml
```

Trong Android Studio, giao diện được xây dựng bằng XML giúp dễ chỉnh sửa và hỗ trợ nhiều thiết bị Android khác nhau.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 17 - Giao diện FoodGuideApp]`

---

## 8. Xử lý dữ liệu JSON

Ứng dụng đọc dữ liệu JSON từ thư mục Assets và xử lý bằng:

* JSONArray
* JSONObject

Sau khi đọc dữ liệu, chương trình sẽ:

1. Hiển thị danh sách món ăn.
2. Lọc món ăn theo tỉnh thành.
3. Tìm kiếm món ăn theo từ khóa người dùng nhập.

Thuật toán xử lý:

* Duyệt JSON.
* Lọc theo province.
* Tìm kiếm theo keyword.
* Hiển thị bằng ListView.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 18 - Code đọc JSON từ Assets]`

---

## 9. Kết quả hoạt động App1

Ứng dụng cho phép:

* Tìm món ăn theo tên.
* Chọn tỉnh thành.
* Hiển thị thông tin chi tiết món ăn.

Giúp người dùng tra cứu dữ liệu món ăn ngay cả khi offline.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 19 - Kết quả hoạt động App1]`

---

# PROJECT 2 - APP2 (MIT TƯƠNG ĐƯƠNG)

## 10. Giới thiệu ứng dụng App2

Ứng dụng App2 được xây dựng tương đương với ứng dụng MIT App Inventor gồm 3 Activity:

* Activity1: About
* Activity2: Giải toán + API
* Activity3: WebView

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 20 - Tạo project App2MitInventor]`

---

## 11. Activity1 - About

Activity1 dùng để:

* Hiển thị thông tin cá nhân.
* Điều hướng sang Activity2.
* Điều hướng sang Activity3.

Sự kiện click Button được xử lý bằng:

```java
Intent intent =
        new Intent(
                MainActivity.this,
                Activity2.class
        );

startActivity(intent);
```

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 21 - Activity1 About]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 22 - Code Intent mở Activity]`

---

## 12. Activity2 - Giải toán + API

Activity2 thực hiện:

* Giải phương trình bậc hai.
* Tính delta.
* Hiển thị nghiệm.
* Gửi dữ liệu lên API.

API sử dụng:

```text
https://k58kmt.tdh.io.vn/api
```

Dữ liệu gửi đi:

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

Dữ liệu trả về:

```json
{
 "ok":1,
 "stt":1234
}
```

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 23 - Giao diện Activity2]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 24 - Code gọi API]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 25 - Kết quả API]`

---

## 13. Activity3 - WebView

Activity3 sử dụng thành phần:

```text
WebView
```

để truy cập website:

```text
https://k58kmt.tdh.io.vn?masv=K225480106064
```

WebView giúp hiển thị website trực tiếp trong ứng dụng mà không cần mở trình duyệt ngoài.

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 26 - Activity3 WebView]`

📷 **Ảnh minh hoạ cần chèn:**
`[ẢNH 27 - Code WebView]`

---

# KẾT LUẬN

Qua bài tập lớn, em đã tìm hiểu được:

* MIT App Inventor
* Android Studio
* WebView
* API JSON
* AndroidManifest.xml
* Activity Lifecycle
* Thư mục Assets
* Xử lý JSON trong Android
* Lập trình Java trên Android

Đồng thời giúp nâng cao kỹ năng xây dựng ứng dụng Android thực tế.

