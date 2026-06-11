# BÀI TẬP LỚN MÔN PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## Thông tin sinh viên

* **Họ và tên:** Hứa Thị Thanh Hiền
* **Mã sinh viên:** K225480106016
* **Lớp:** K58KTP
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

![Ảnh 1](images/1.png)

---

### **Viewer**

Là khu vực hiển thị giao diện ứng dụng mô phỏng điện thoại Android.

Người dùng kéo thả các thành phần từ Palette sang Viewer để xây dựng giao diện.

![Ảnh 2](images/2.png)

---

### **Components**

Hiển thị danh sách các đối tượng đang tồn tại trong ứng dụng như:

* Button
* Label
* WebViewer
* Screen

Cho phép đổi tên hoặc quản lý thành phần.

![Ảnh 3](images/3.png)

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

![Ảnh 4](images/4.png)

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

![Ảnh 5](images/5.png)

---

### 3.2 Block Programming là gì?

Block Programming là phương pháp lập trình trực quan bằng cách ghép các khối lệnh.

Ví dụ:

* Khi nhấn Button → thực hiện phép tính.
* Khi mở Screen → mở website.

Khối lệnh sẽ được ghép nối như các mảnh ghép logic.

![Ảnh 6](images/6.png)

![Ảnh 7](images/7.png)

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

![Ảnh 8](images/8.png)

---

## 4. Thiết kế ứng dụng MIT App Inventor

### 4.1 Screen1 - About

Màn hình giới thiệu thông tin sinh viên gồm:

* Họ tên
* Mã sinh viên
* Nút mở Screen2
* Nút mở Screen3

![Ảnh 9](images/9.png)

---

### 4.2 Screen2 - Giải toán đơn giản

Ứng dụng xây dựng chức năng giải phương trình đơn giản.

Người dùng nhập dữ liệu và nhấn nút tính để hiển thị kết quả.

![Ảnh 10](images/10.png)

![Ảnh 11](images/11.jpg)

---

### 4.3 Screen3 - WebViewer

Sử dụng **WebViewer** để hiển thị website:

```text
https://k58kmt.tdh.io.vn?masv=K225480106064
```

Website được tối ưu cho giao diện điện thoại.

![Ảnh 12](images/12.jpg)

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

![Ảnh 13](images/13.png)

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

![Ảnh 14](images/14.png)

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

![Ảnh 15](images/15.png)

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

![Ảnh 16](images/16.png)

## 7. Giao diện ứng dụng App1

![Ảnh 17](images/17.png)

## 8. Xử lý dữ liệu JSON

![Ảnh 18](images/18.png)

## 9. Kết quả hoạt động App1

![Ảnh 19](images/19.png)

# PROJECT 2 - APP2 (MIT TƯƠNG ĐƯƠNG)

## 10. Giới thiệu ứng dụng App2

![Ảnh 20](images/20.png)

## 11. Activity1 - About

![Ảnh 21](images/21.png)

![Ảnh 22](images/22.png)

## 12. Activity2 - Giải toán + API

![Ảnh 23](images/23.png)

![Ảnh 24](images/24.png)

![Ảnh 25](images/25.png)

## 13. Activity3 - WebView

![Ảnh 26](images/26.png)

![Ảnh 27](images/27.png)

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
