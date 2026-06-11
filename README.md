# BÀI TẬP LỚN MÔN PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## Thông tin sinh viên

* **Họ và tên:** Hứa Thị Thanh Hiền
* **Mã sinh viên:** K225480106016
* **Lớp:** K58KTP
* **Môn học:** Phát triển ứng dụng trên thiết bị di động - TEE0419

---

# PHẦN 1: ỨNG DỤNG MIT APP INVENTOR

## 1. Mục tiêu chương trình

Trong phần đầu của bài tập lớn, em tiến hành xây dựng ứng dụng trên nền tảng **MIT App Inventor** nhằm làm quen với quy trình phát triển ứng dụng Android bằng phương pháp kéo thả (**Drag and Drop**).

Ứng dụng được xây dựng gồm **3 màn hình (Screen)** với các chức năng cụ thể như sau:

* **Screen1:** Giới thiệu thông tin bản thân và điều hướng sang các màn hình khác.
* **Screen2:** Giải một bài toán đơn giản (phương trình bậc hai).
* **Screen3:** Hiển thị website bằng **WebViewer**.

Thông qua ứng dụng này, em có cơ hội tìm hiểu:

* Quy trình thiết kế giao diện trên MIT App Inventor.
* Cơ chế kéo thả thành phần giao diện.
* Lập trình bằng Block Programming.
* Điều hướng giữa nhiều màn hình.
* Xử lý dữ liệu nhập từ người dùng.

Ứng dụng được phát triển bằng phương pháp kéo thả giúp người dùng không cần viết nhiều mã lệnh nhưng vẫn có thể xây dựng được ứng dụng Android cơ bản.

---

## 2. Thiết kế giao diện MIT App Inventor

### 2.1 Thanh công cụ trong MIT App Inventor

Trong quá trình phát triển ứng dụng, MIT App Inventor cung cấp nhiều khu vực làm việc chính nhằm hỗ trợ người dùng thiết kế giao diện và lập trình trực quan.

### **Palette**

Palette là nơi chứa các thành phần giao diện và chức năng có thể sử dụng trong ứng dụng.

Một số thành phần thường dùng bao gồm:

* Button
* Label
* TextBox
* WebViewer
* Horizontal Arrangement
* Vertical Arrangement

Người dùng có thể kéo thả trực tiếp các thành phần từ Palette vào màn hình thiết kế.

Chức năng của Palette:

* Hỗ trợ thiết kế nhanh giao diện.
* Giúp tìm kiếm và lựa chọn component.
* Hạn chế việc viết code thủ công.

![Ảnh 1](images/1.png)

---

### **Viewer**

Viewer là khu vực hiển thị mô phỏng giao diện ứng dụng trên điện thoại Android.

Người dùng có thể kéo thả các thành phần từ **Palette** sang **Viewer** để thiết kế bố cục ứng dụng theo ý muốn.

Nhờ Viewer, quá trình xây dựng giao diện trở nên trực quan hơn, người lập trình có thể quan sát ngay cách hiển thị của ứng dụng mà không cần chạy thử nhiều lần.

![Ảnh 2](images/2.png)

---

### **Components**

Components là khu vực quản lý toàn bộ thành phần đã được thêm vào ứng dụng.

Ví dụ:

* Button
* Label
* WebViewer
* Screen

Tại đây người dùng có thể:

* Đổi tên component.
* Quản lý đối tượng.
* Theo dõi cấu trúc ứng dụng.

Việc đổi tên component giúp quá trình lập trình bằng block dễ quản lý hơn, tránh nhầm lẫn giữa nhiều đối tượng.

![Ảnh 3](images/3.png)

---

### **Properties**

Properties cho phép chỉnh sửa thuộc tính của từng thành phần.

Ví dụ:

* Width
* Height
* Text
* Font Size
* Background Color
* Text Color

Người dùng có thể dễ dàng thay đổi màu sắc, kích thước hoặc nội dung hiển thị mà không cần viết code.

Ví dụ:

* Đổi màu Button.
* Thay đổi kích thước chữ.
* Chỉnh vị trí hiển thị.

![Ảnh 4](images/4.png)

---

## 3. Cơ chế kéo thả và Block Programming

### 3.1 Kéo thả giao diện

MIT App Inventor hoạt động theo cơ chế kéo thả (**Drag and Drop**).

Người dùng chỉ cần:

1. Chọn thành phần trong **Palette**
2. Kéo vào **Viewer**
3. Chỉnh thuộc tính trong **Properties**

Ví dụ trong ứng dụng:

* Kéo **Button** để tạo nút chuyển màn hình.
* Kéo **Label** để hiển thị thông tin cá nhân.
* Kéo **TextBox** để nhập hệ số phương trình.
* Kéo **WebViewer** để hiển thị website.

Cơ chế này giúp việc xây dựng giao diện trở nên nhanh chóng và phù hợp với người mới học lập trình.

![Ảnh 5](images/5.png)

---

### 3.2 Block Programming là gì?

Block Programming là phương pháp lập trình trực quan bằng cách ghép các khối lệnh logic thay vì viết code bằng văn bản.

Mỗi block sẽ đại diện cho một hành động cụ thể và được ghép nối với nhau giống như các mảnh ghép.

Ví dụ:

* Khi nhấn Button → mở màn hình mới.
* Khi nhấn nút tính → thực hiện phép toán.
* Khi mở Screen → tải website.

Trong ứng dụng, block được sử dụng để:

* Chuyển giữa các màn hình.
* Xử lý phương trình bậc hai.
* Hiển thị kết quả.

Khối lệnh giúp người học dễ hình dung tư duy logic hơn so với lập trình truyền thống.

![Ảnh 6](images/6.png)

![Ảnh 7](images/7.png)

---

### 3.3 Ưu điểm của Block so với viết Code

**Ưu điểm:**

* Dễ học.
* Không cần nhớ cú pháp.
* Hạn chế lỗi cú pháp.
* Tốc độ phát triển nhanh.
* Phù hợp với người mới học lập trình.

**Nhược điểm:**

* Khó mở rộng với dự án lớn.
* Ít linh hoạt hơn Java/Kotlin.
* Giao diện block dễ rối khi ứng dụng phức tạp.

Tuy nhiên đối với mục đích học tập và xây dựng ứng dụng đơn giản thì MIT App Inventor là công cụ rất phù hợp.

---

### 3.4 Backpack (Copy/Paste Block)

Backpack là chức năng hỗ trợ sao chép và tái sử dụng block giữa nhiều screen khác nhau.

Backpack giúp:

* Copy block.
* Paste block.
* Tái sử dụng logic xử lý.
* Tiết kiệm thời gian lập trình.

Ví dụ:

Nếu đã tạo block chuyển màn hình ở Screen1 thì có thể sao chép sang các Screen khác mà không cần làm lại từ đầu.

![Ảnh 8](images/8.png)

---

## 4. Thiết kế ứng dụng MIT App Inventor

### 4.1 Screen1 - About

Screen1 đóng vai trò là màn hình chính của ứng dụng.

Màn hình này được sử dụng để giới thiệu thông tin sinh viên và điều hướng sang các chức năng khác.

Thông tin hiển thị gồm:

* Họ tên sinh viên.
* Mã sinh viên.
* Lớp học.

Ngoài ra còn có:

* Nút mở **Screen2** để giải toán.
* Nút mở **Screen3** để hiển thị website.

Khi người dùng nhấn nút tương ứng, ứng dụng sẽ tự động chuyển sang màn hình chức năng.

![Ảnh 9](images/9.png)

---

### 4.2 Screen2 - Giải toán đơn giản

Ứng dụng xây dựng chức năng giải phương trình bậc hai theo dạng:

ax² + bx + c = 0

Người dùng nhập:

* Hệ số a
* Hệ số b
* Hệ số c

sau đó nhấn nút **GIẢI** để chương trình xử lý.

Ứng dụng sẽ tính giá trị Delta và xét các trường hợp:

* Δ < 0 → vô nghiệm
* Δ = 0 → nghiệm kép
* Δ > 0 → hai nghiệm phân biệt

Kết quả sau khi tính toán sẽ được hiển thị trên màn hình thông qua Label.

![Ảnh 10](images/10.png)

![Ảnh 11](images/11.jpg)

---

### 4.3 Screen3 - WebViewer

Screen3 sử dụng thành phần **WebViewer** để hiển thị website trực tiếp bên trong ứng dụng.

Website sử dụng:

```text
https://k58kmt.tdh.io.vn?masv=K225480106016
```

WebViewer giúp:

* Hiển thị website mà không cần mở trình duyệt ngoài.
* Tối ưu hiển thị trên điện thoại.
* Mang lại trải nghiệm liền mạch cho người dùng.

Màn hình này được sử dụng nhằm phục vụ kiểm tra thông tin sinh viên dựa trên mã số sinh viên.

![Ảnh 12](images/12.jpg)

# PHẦN 2: ỨNG DỤNG ANDROID STUDIO

## 1. Giới thiệu

Sau khi hoàn thành ứng dụng trên nền tảng **MIT App Inventor**, em tiếp tục xây dựng ứng dụng tương đương bằng **Android Studio** nhằm hiểu rõ hơn về lập trình ứng dụng Android bằng ngôn ngữ Java.

Android Studio là môi trường phát triển ứng dụng Android chính thức do Google cung cấp. So với MIT App Inventor, Android Studio có tính linh hoạt cao hơn, cho phép lập trình viên kiểm soát sâu hơn về giao diện, dữ liệu và hiệu năng ứng dụng.

Ứng dụng Android Studio được xây dựng tương đương với MIT App Inventor gồm **3 Activity**:

* **Activity1:** About – giới thiệu thông tin sinh viên.
* **Activity2:** Giải toán + gọi API.
* **Activity3:** WebView hiển thị website.

Ngoài ra, em còn thực hiện thêm **App1 - Food Guide App** nhằm thực hành kỹ năng xử lý dữ liệu JSON, đọc file từ thư mục Assets và hiển thị dữ liệu offline.

---

## 2. Tạo Project Android Studio

Tiến hành mở Android Studio và tạo project mới bằng ngôn ngữ Java.

Template sử dụng:

```text id="t9nsu0"
Empty Views Activity
```

Sau khi tạo project, Android Studio sẽ tự động sinh ra các file cơ bản như:

* `MainActivity.java`
* `activity_main.xml`
* `AndroidManifest.xml`

Cùng với các thư mục quan trọng:

* `java` – chứa mã nguồn Java.
* `res` – chứa giao diện và tài nguyên.
* `drawable` – chứa hình ảnh.
* `layout` – chứa file giao diện XML.
* `values` – chứa string, màu sắc, theme.

Việc sử dụng Java giúp ứng dụng dễ xử lý logic và tương thích tốt với Android Studio.

![Ảnh 13](images/13.png)

---

## 3. AndroidManifest.xml

### Chức năng

File `AndroidManifest.xml` là file rất quan trọng trong Android.

File này dùng để:

* Khai báo Activity.
* Khai báo quyền ứng dụng.
* Xác định màn hình khởi động.
* Quản lý cấu hình ứng dụng.

Ví dụ khai báo quyền Internet:

```xml id="h5pfm5"
<uses-permission
    android:name="android.permission.INTERNET"/>
```

Mục đích:

Cho phép ứng dụng:

* Kết nối API.
* Hiển thị website bằng WebView.
* Gửi dữ liệu lên server.

Nếu không khai báo quyền Internet, ứng dụng sẽ không thể truy cập dữ liệu từ website hoặc API.

Ngoài ra, trong Manifest còn khai báo các Activity:

* `MainActivity`
* `MainActivity2`
* `MainActivity3`

để Android biết ứng dụng có những màn hình nào.

![Ảnh 14](images/14.png)

---

## 4. Vòng đời ứng dụng Android

Một Activity Android có các trạng thái chính:

* `onCreate()`
* `onStart()`
* `onResume()`
* `onPause()`
* `onStop()`
* `onDestroy()`

### onCreate()

Đây là hàm đầu tiên được chạy khi Activity được tạo.

Android Studio tự động sinh hàm này sau khi tạo project vì đây là nơi dùng để khởi tạo giao diện và xử lý logic ban đầu.

Ví dụ:

```java id="mjlwmv"
setContentView(R.layout.activity_main);
```

Có nhiệm vụ gắn giao diện XML vào màn hình.

Ngoài ra còn dùng:

```java id="b2q7c4"
findViewById()
```

để ánh xạ View.

Ví dụ:

```java id="3v6w3i"
Button btnMath =
findViewById(R.id.btnMath);
```

### onStart()

Được gọi khi Activity bắt đầu hiển thị.

### onResume()

Cho phép người dùng tương tác trực tiếp với ứng dụng.

### onPause()

Được gọi khi ứng dụng tạm thời mất focus.

Ví dụ:

* Có cuộc gọi đến.
* Người dùng chuyển app.

### onStop()

Activity không còn hiển thị.

### onDestroy()

Activity bị đóng hoàn toàn.

Hiểu vòng đời Activity giúp lập trình viên tối ưu hiệu năng và quản lý dữ liệu hiệu quả hơn.

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

```text id="rm8b4f"
foods.json
```

và đặt trong thư mục:

```text id="6np7mq"
app/src/main/assets
```

Khi build APK, toàn bộ file trong Assets sẽ được đóng gói cùng ứng dụng.

Điều này giúp ứng dụng hoạt động được ngay cả khi không có Internet.

![Ảnh 16](images/16.png)

---

## 6. Giao diện ứng dụng App1

Ứng dụng Food Guide được thiết kế với giao diện đơn giản và thân thiện với người dùng.

Các thành phần chính gồm:

* **EditText** – nhập từ khóa tìm kiếm.
* **Spinner** – lọc theo tỉnh thành.
* **ListView** – hiển thị danh sách món ăn.
* **TextView** – hiển thị thông tin chi tiết.

Người dùng có thể chọn món ăn để xem:

* Tên món ăn.
* Tỉnh thành.
* Mô tả.
* Thành phần nguyên liệu.

Việc sử dụng ListView giúp dữ liệu hiển thị rõ ràng và dễ thao tác.

![Ảnh 17](images/17.png)

---

## 7. Xử lý dữ liệu JSON

Ứng dụng sử dụng dữ liệu từ file:

```text id="4f0jlwm"
foods.json
```

Android hỗ trợ đọc file từ Assets bằng cú pháp:

```java id="aqz7yx"
getAssets().open("foods.json");
```

Sau khi đọc dữ liệu, ứng dụng sử dụng:

```java id="mjlwm6"
JSONArray
```

để xử lý danh sách món ăn.

Dữ liệu được duyệt bằng vòng lặp:

```java id="ffk5nm"
for(int i=0;i<jsonArray.length();i++)
```

Sau đó hiển thị dữ liệu lên giao diện.

Ưu điểm của JSON:

* Nhẹ.
* Dễ đọc.
* Dễ mở rộng dữ liệu.
* Tương thích tốt với Android.

![Ảnh 18](images/18.png)

---

## 8. Kết quả hoạt động App1

Sau khi chạy ứng dụng, dữ liệu món ăn được hiển thị chính xác.

Người dùng có thể:

* Xem danh sách món ăn.
* Chọn tỉnh thành.
* Xem mô tả chi tiết.
* Sử dụng ứng dụng khi không có mạng.

Việc dùng Assets giúp tốc độ tải dữ liệu nhanh hơn so với việc gọi API trực tiếp từ Internet.

![Ảnh 19](images/19.png)

# PROJECT 2 - APP2 (MIT TƯƠNG ĐƯƠNG)

## 9. Giới thiệu ứng dụng App2

Ứng dụng App2 được xây dựng nhằm mô phỏng lại ứng dụng đã thực hiện bằng MIT App Inventor nhưng phát triển bằng Android Studio.

Ứng dụng gồm:

* Activity1: About.
* Activity2: Giải toán.
* Activity3: WebView.

Mục tiêu:

* Hiểu cách viết ứng dụng Android bằng Java.
* Xử lý sự kiện Button.
* Chuyển màn hình bằng Intent.
* Gọi API và WebView.

![Ảnh 20](images/20.png)

## 10. Activity1 - About

### Thiết kế giao diện

Activity1 đóng vai trò là màn hình chính của ứng dụng.

Màn hình này có chức năng giới thiệu thông tin cá nhân của sinh viên và điều hướng sang các Activity khác.

Thông tin hiển thị gồm:

* Họ và tên sinh viên.
* Mã sinh viên.
* Lớp học.

Ngoài ra, màn hình còn có hai nút chức năng:

* **Bài Toán** → chuyển sang Activity giải phương trình.
* **Web** → chuyển sang Activity hiển thị website.

Giao diện được thiết kế bằng file XML trong thư mục:

```text id="z1m7h4"
res/layout
```

Android Studio cho phép xây dựng giao diện bằng cách kéo thả hoặc viết trực tiếp XML.

Trong quá trình thiết kế giao diện, em sử dụng các thành phần:

* **TextView** – hiển thị nội dung văn bản.
* **Button** – tạo nút bấm.
* **LinearLayout** – sắp xếp giao diện.

Thuộc tính:

```xml id="3r8g5v"
android:orientation="vertical"
```

được sử dụng để sắp xếp các đối tượng theo chiều dọc.

Ngoài ra còn có:

```xml id="zjlwm5"
android:gravity="center"
```

giúp căn giữa giao diện.

![Ảnh 21](images/21.png)

---

### Xử lý sự kiện Activity1

Sau khi hoàn thiện giao diện, em tiến hành viết code xử lý sự kiện khi người dùng nhấn Button.

Trong Android, khi muốn xử lý sự kiện nhấn nút, có thể sử dụng:

### Cách 1: setOnClickListener()

Đây là cách được sử dụng trong bài tập.

Ví dụ:

```java id="jlwm9q"
btnMath.setOnClickListener(v -> {
});
```

Khi người dùng nhấn nút, chương trình sẽ thực hiện hành động tương ứng.

Để chuyển màn hình Android, em sử dụng:

```java id="3jlwmz"
Intent intent =
new Intent(
MainActivity.this,
MainActivity2.class
);
```

sau đó gọi:

```java id="jlwmw2"
startActivity(intent);
```

### Cách 2: android:onClick

Có thể khai báo trực tiếp trong XML:

```xml id="jlwm6h"
android:onClick="openScreen"
```

Tuy nhiên cách này ít linh hoạt hơn nên em lựa chọn `setOnClickListener()`.

Ngoài ra, trong Android Studio, hàm:

```java id="jlwm1n"
onCreate()
```

được tự động sinh ra sau khi tạo project vì đây là hàm đầu tiên chạy khi Activity khởi tạo.

![Ảnh 22](images/22.png)

---

## 11. Activity2 - Giải toán + API

### Thiết kế giao diện

Activity2 được xây dựng nhằm giải phương trình bậc hai theo công thức:

Người dùng nhập:

* Hệ số a
* Hệ số b
* Hệ số c

Sau đó nhấn nút:

```text id="jlwm8b"
GIẢI
```

Ứng dụng sẽ thực hiện tính toán và hiển thị kết quả nghiệm.

Các thành phần giao diện gồm:

* **EditText** – nhập hệ số.
* **Button** – xử lý phép tính.
* **TextView** – hiển thị kết quả.

![Ảnh 23](images/23.png)

---

### Xử lý logic giải toán

Sau khi người dùng nhập dữ liệu, ứng dụng sử dụng:

```java id="jlwm4d"
Double.parseDouble()
```

để chuyển dữ liệu từ chuỗi sang kiểu số thực.

Tiếp theo, chương trình tính Delta:

\Delta=b^2-4ac

Sau đó xét các trường hợp:

### Trường hợp 1: Δ < 0

Phương trình vô nghiệm.

### Trường hợp 2: Δ = 0

Phương trình có nghiệm kép:

x=\frac{-b}{2a}

### Trường hợp 3: Δ > 0

Phương trình có hai nghiệm phân biệt:

x_1=\frac{-b+\sqrt{\Delta}}{2a}

x_2=\frac{-b-\sqrt{\Delta}}{2a}

Kết quả được hiển thị thông qua `TextView`.

![Ảnh 24](images/24.png)

---

### Gọi API sau khi giải toán

Sau khi giải xong bài toán, ứng dụng tiến hành gửi dữ liệu lên API:

```text id="jlwm7r"
https://k58kmt.tdh.io.vn/api
```

Dữ liệu gửi lên gồm:

```json id="jlwm0v"
{
 "app_by":"K225480106016",
 "input":{
   "a":1,
   "b":2,
   "c":3
 },
 "output":{
   "ketluan":"Vo nghiem"
 }
}
```

Ứng dụng sử dụng thư viện **Volley** để gửi request HTTP dạng JSON.

Sau khi gửi thành công, hệ thống phản hồi:

```json id="jlwm3m"
{
 "ok":1,
 "stt":1234
}
```

Giúp xác nhận dữ liệu đã được gửi thành công.

![Ảnh 25](images/25.png)

---

## 12. Activity3 - WebView

### Giới thiệu chức năng

Activity3 sử dụng thành phần **WebView** để hiển thị website trực tiếp bên trong ứng dụng Android.

Website sử dụng:

```text id="jlwm2y"
https://k58kmt.tdh.io.vn?masv=K225480106016
```

Để sử dụng WebView, ứng dụng cần khai báo quyền:

```xml id="jlwm6g"
android.permission.INTERNET
```

trong file `AndroidManifest.xml`.

![Ảnh 26](images/26.png)

---

### Xử lý WebView bằng Java

Trong Java, em thực hiện khai báo:

```java id="jlwm8p"
WebView webView;
```

Sau đó cấu hình:

```java id="jlwm1g"
webView.getSettings()
.setJavaScriptEnabled(true);
```

Giúp website hiển thị đầy đủ nội dung.

Để tránh mở trình duyệt ngoài, em sử dụng:

```java id="jlwm5d"
webView.setWebViewClient(
new WebViewClient()
);
```

Cuối cùng dùng:

```java id="jlwm9f"
webView.loadUrl()
```

để tải website theo mã sinh viên.

Kết quả hiển thị chính xác thông tin sinh viên như:

* Họ tên.
* Mã sinh viên.
* Ngày sinh.
* Bộ đếm truy cập.

![Ảnh 27](images/27.png)

---

# KẾT LUẬN

Qua bài tập lớn môn **Phát triển ứng dụng trên thiết bị di động - TEE0419**, em đã tìm hiểu và thực hành được nhiều kiến thức quan trọng trong phát triển ứng dụng Android.

Các kiến thức đã học gồm:

* MIT App Inventor.
* Android Studio.
* Java Language.
* Block Programming.
* XML Layout.
* AndroidManifest.xml.
* Activity Lifecycle.
* Intent.
* WebView.
* API JSON.
* Volley.
* Thư mục Assets.
* Xử lý JSON trong Android.

Thông qua bài tập, em hiểu rõ hơn quy trình xây dựng ứng dụng Android từ thiết kế giao diện, xử lý logic đến triển khai chức năng thực tế.

Đồng thời, bài tập giúp em nâng cao kỹ năng lập trình Java, khả năng xử lý dữ liệu và phát triển ứng dụng Android có tính ứng dụng thực tế.
