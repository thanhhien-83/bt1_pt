# MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## 1. Giới thiệu

Sau khi hoàn thành ứng dụng bằng **MIT App Inventor**, em tiếp tục xây dựng ứng dụng tương đương bằng **Android Studio** sử dụng ngôn ngữ lập trình **Java**.

Android Studio là môi trường phát triển ứng dụng Android chính thức do Google cung cấp. So với MIT App Inventor, Android Studio cho phép lập trình linh hoạt hơn, mở rộng chức năng tốt hơn và phù hợp với các dự án thực tế.

Ứng dụng Android Studio trong bài tập lớn gồm:

* **Activity1:** Giới thiệu thông tin cá nhân và điều hướng.
* **Activity2:** Giải phương trình bậc hai và hiển thị kết quả.
* **Activity3:** Hiển thị website bằng **WebView**.

Ngoài ra, em còn xây dựng thêm **App1 - Food Guide App** sử dụng dữ liệu JSON lưu trong thư mục **Assets** nhằm minh họa khả năng xử lý dữ liệu offline trên Android.

---

## 2. Tạo Project Android Studio

Đầu tiên, em tiến hành mở **Android Studio** và tạo project mới.

Template được sử dụng:

```text
Empty Views Activity
```

Project được tạo bằng ngôn ngữ:

```text
Java
```

Sau khi tạo project, Android Studio sẽ tự sinh sẵn cấu trúc thư mục và các file quan trọng như:

* `MainActivity.java`
* `activity_main.xml`
* `AndroidManifest.xml`
* thư mục `res`
* thư mục `java`

Ngoài ra, hệ thống Gradle sẽ tự động quản lý thư viện và quá trình build ứng dụng Android.

![Ảnh 13](images/13.png)

---

## 3. AndroidManifest.xml

### 3.1 Chức năng của AndroidManifest.xml

File `AndroidManifest.xml` đóng vai trò rất quan trọng trong ứng dụng Android.

File này dùng để:

* Khai báo Activity.
* Khai báo quyền của ứng dụng.
* Thiết lập launcher app.
* Khai báo theme ứng dụng.
* Quản lý cấu hình tổng thể của app.

Trong bài tập lớn, ứng dụng cần truy cập website và gọi API nên cần cấp quyền truy cập Internet.

Do đó em khai báo:

```xml
<uses-permission
    android:name="android.permission.INTERNET"/>
```

Ý nghĩa:

Cho phép ứng dụng kết nối Internet để:

* gọi API.
* sử dụng WebView.
* hiển thị website trực tiếp trong ứng dụng.

Nếu không khai báo quyền này thì ứng dụng sẽ không thể truy cập dữ liệu từ Internet.

Ngoài ra trong file Manifest còn khai báo các **Activity** của ứng dụng:

* `MainActivity`
* `MainActivity2`
* `MainActivity3`

Giúp Android biết màn hình nào sẽ được mở khi người dùng sử dụng app.

![Ảnh 14](images/14.png)

---

## 4. Vòng đời ứng dụng Android

Trong Android, mỗi Activity đều có một vòng đời hoạt động gọi là **Activity Lifecycle**.

Các trạng thái chính bao gồm:

### **onCreate()**

Đây là hàm đầu tiên được gọi khi Activity được khởi tạo.

Hàm này thường dùng để:

* Khởi tạo giao diện.
* Ánh xạ View bằng `findViewById()`.
* Khởi tạo dữ liệu.
* Viết logic ban đầu.

Ví dụ:

```java
setContentView(R.layout.activity_main);
```

Dùng để gắn giao diện XML vào màn hình.

Android Studio tự sinh sẵn `onCreate()` khi tạo project vì đây là hàm bắt buộc để khởi tạo Activity.

---

### **onStart()**

Được gọi khi Activity bắt đầu hiển thị với người dùng.

---

### **onResume()**

Activity bắt đầu tương tác trực tiếp với người dùng.

---

### **onPause()**

Được gọi khi Activity tạm thời mất focus.

Ví dụ:

* Có cuộc gọi đến.
* Người dùng chuyển ứng dụng.

---

### **onStop()**

Activity không còn hiển thị trên màn hình.

---

### **onDestroy()**

Được gọi khi Activity bị đóng hoàn toàn.

Việc hiểu vòng đời ứng dụng giúp lập trình viên tối ưu hiệu năng và xử lý dữ liệu phù hợp khi chuyển đổi màn hình.

![Ảnh 15](images/15.png)

---

# PROJECT 1 - APP1 (FOOD GUIDE APP)

## 5. Giới thiệu ứng dụng App1

Đây là ứng dụng được xây dựng nhằm minh họa cơ chế lưu dữ liệu sẵn trong Android thông qua thư mục **Assets**.

Ý tưởng của ứng dụng:

Xây dựng một chương trình giúp người dùng tìm hiểu các món ăn đặc trưng của Việt Nam theo từng tỉnh thành.

Chức năng của ứng dụng gồm:

* Hiển thị danh sách món ăn.
* Lọc món ăn theo khu vực.
* Hiển thị thông tin chi tiết.
* Hoạt động offline không cần Internet.

Dữ liệu được lưu sẵn dưới dạng file:

```text
foods.json
```

và đặt trong thư mục:

```text
app/src/main/assets
```

Việc sử dụng Assets giúp dữ liệu luôn đi theo ứng dụng sau khi build APK.

Ngay cả khi không có mạng Internet thì người dùng vẫn sử dụng được ứng dụng.

![Ảnh 16](images/16.png)

---

## 6. Cấu trúc dữ liệu JSON

Ứng dụng sử dụng file `foods.json` để lưu thông tin món ăn.

Mỗi món ăn gồm các thuộc tính:

* `name` – tên món ăn.
* `province` – tỉnh thành.
* `description` – mô tả.
* `ingredients` – nguyên liệu.

Ví dụ:

```json
{
   "name":"Phở",
   "province":"Hà Nội",
   "description":"Món ăn truyền thống nổi tiếng",
   "ingredients":"Bánh phở, thịt bò, nước dùng"
}
```

Một số món ăn được thêm vào:

* Phở
* Bún bò Huế
* Bánh mì

Việc sử dụng JSON giúp:

* Dễ quản lý dữ liệu.
* Dễ mở rộng.
* Nhẹ và tối ưu cho mobile app.
* Dễ đọc dữ liệu bằng Java.

![Ảnh 17](images/17.png)

---

## 7. Xử lý dữ liệu JSON trong Android

Sau khi tạo file JSON, em tiến hành đọc dữ liệu từ thư mục **Assets**.

Android hỗ trợ truy cập file Assets bằng cú pháp:

```java
getAssets().open("foods.json")
```

Dữ liệu được đọc thành chuỗi JSON và chuyển sang `JSONArray` để xử lý.

Sau đó ứng dụng sử dụng vòng lặp:

```java
for(int i = 0; i < jsonArray.length(); i++)
```

để đọc từng món ăn và thêm vào danh sách hiển thị.

Các đối tượng sử dụng trong ứng dụng gồm:

* **ListView** – hiển thị danh sách món ăn.
* **Spinner** – lọc theo tỉnh thành.
* **TextView** – hiển thị thông tin chi tiết.

Việc xử lý dữ liệu JSON giúp em hiểu rõ cách:

* Đọc dữ liệu offline.
* Chuyển đổi JSON sang object.
* Hiển thị dữ liệu trong giao diện Android.

![Ảnh 18](images/18.png)

---

## 8. Kết quả hoạt động App1

Sau khi chạy chương trình, ứng dụng hiển thị thành công danh sách món ăn.

Người dùng có thể:

* Chọn món ăn.
* Xem thông tin chi tiết.
* Quan sát nguyên liệu và mô tả món ăn.

Ví dụ:

Khi chọn **Phở**, ứng dụng hiển thị:

* Tên món: Phở
* Tỉnh: Hà Nội
* Mô tả: Món ăn truyền thống nổi tiếng
* Nguyên liệu: Bánh phở, thịt bò, nước dùng

Ứng dụng hoạt động hoàn toàn offline nhờ dữ liệu được chuẩn bị sẵn trong thư mục Assets.

Điều này giúp:

* Không phụ thuộc Internet.
* Tăng tốc độ tải dữ liệu.
* Dễ triển khai ứng dụng thực tế.

![Ảnh 19](images/19.png)

# PROJECT 2 - APP2 (MIT TƯƠNG ĐƯƠNG)

## 9. Giới thiệu ứng dụng App2

Sau khi hoàn thành ứng dụng bằng **MIT App Inventor**, em tiếp tục xây dựng lại ứng dụng tương đương bằng **Android Studio** nhằm hiểu rõ hơn về lập trình Android bằng ngôn ngữ Java.

Ứng dụng App2 được xây dựng gồm **3 Activity** tương ứng với 3 Screen trong MIT App Inventor:

* **Activity1:** Giới thiệu bản thân và điều hướng.
* **Activity2:** Giải phương trình bậc hai.
* **Activity3:** Hiển thị website bằng WebView.

Mục tiêu của ứng dụng:

* Hiểu quy trình phát triển app Android thực tế.
* Làm quen với XML Layout.
* Xử lý sự kiện Button.
* Chuyển màn hình bằng Intent.
* Hiển thị website bằng WebView.
* Thực hiện xử lý dữ liệu đầu vào.

Ứng dụng được xây dựng bằng **Java Language** kết hợp với giao diện XML.

![Ảnh 20](images/20.png)

---

## 10. Activity1 - About

### 10.1 Thiết kế giao diện

Activity1 đóng vai trò là màn hình chính của ứng dụng.

Màn hình này được thiết kế gồm:

* Họ và tên sinh viên.
* Mã sinh viên.
* Lớp học.
* Nút mở màn hình giải toán.
* Nút mở màn hình website.

Giao diện được xây dựng bằng file XML trong thư mục:

```text id="h6z9gb"
res/layout
```

Trong Android, giao diện được mô tả bằng ngôn ngữ **XML** thay vì kéo thả như MIT App Inventor.

Ví dụ:

```xml id="z3tt0q"
<TextView
    android:text="Hứa Thanh Hiền"/>
```

Tuy nhiên trong Android Studio, việc hardcode text như trên không được khuyến khích.

Thông thường giá trị text nên lưu trong:

```text id="0wpwwr"
res/values/strings.xml
```

và tham chiếu bằng cú pháp:

```xml id="t0l7v2"
android:text="@string/app_name"
```

### Ưu điểm của việc tham chiếu String Resource

* Dễ thay đổi nội dung.
* Hỗ trợ đa ngôn ngữ.
* Android tự động hiển thị theo ngôn ngữ hệ thống.
* Hỗ trợ Theme và Dark Mode.

Ví dụ:

Nếu điện thoại sử dụng tiếng Anh thì hệ thống sẽ tự lấy nội dung trong thư mục:

```text id="viy5qe"
values-en
```

Nếu là tiếng Việt sẽ dùng:

```text id="luw91z"
values-vi
```

Điều này giúp ứng dụng có khả năng hỗ trợ quốc tế hóa (**Localization**).

Ngoài ra, giao diện còn sử dụng:

### **LinearLayout**

Đây là đối tượng dùng để chứa các thành phần con.

Trong bài tập:

```xml id="lwl5e4"
android:orientation="vertical"
```

Giúp sắp xếp các thành phần theo chiều dọc.

Có thể sử dụng:

```xml id="8q0kr7"
horizontal
```

để sắp xếp theo chiều ngang.

Ngoài ra thuộc tính:

```xml id="3lt1l9"
gravity
```

dùng để căn chỉnh nội dung:

* left
* right
* center

![Ảnh 21](images/21.png)

---

### 10.2 Code xử lý Activity1

Sau khi thiết kế giao diện XML, em tiến hành xử lý sự kiện cho các nút bấm.

Trong Android, sự kiện người dùng như:

* Click Button
* Click Text
* Touch màn hình

được gọi là **Event**.

Có hai cách xử lý Event phổ biến:

### Cách 1: `setOnClickListener()`

Đây là cách em sử dụng trong bài tập.

Ví dụ:

```java id="5g6fku"
btnMath.setOnClickListener(v -> {
});
```

Khi người dùng nhấn Button, đoạn code bên trong sẽ được thực thi.

Trong bài tập:

* `btnMath` → mở Activity giải toán.
* `btnWeb` → mở Activity WebView.

Để chuyển màn hình Android, em sử dụng:

```java id="xh6c95"
Intent intent =
new Intent(MainActivity.this,
MainActivity2.class);
```

Sau đó gọi:

```java id="1rxgzc"
startActivity(intent);
```

### Cách 2: `android:onClick`

Có thể khai báo trực tiếp trong XML:

```xml id="p5o8q4"
android:onClick="openScreen"
```

và viết hàm trong Java:

```java id="2yx9h2"
public void openScreen(View view)
```

Tuy nhiên cách này ít linh hoạt hơn nên em lựa chọn `setOnClickListener()`.

Ngoài ra, Android Studio tự sinh hàm:

```java id="3wbjlwm"
onCreate()
```

sau khi tạo project vì đây là hàm đầu tiên chạy khi Activity khởi tạo.

Trong hàm này thường dùng để:

* Gắn giao diện XML.
* Ánh xạ View.
* Viết logic khởi tạo.

Ví dụ:

```java id="v3p2rt"
setContentView(R.layout.activity_main);
```

và:

```java id="52tp0x"
findViewById()
```

để ánh xạ Button/TextView.

![Ảnh 22](images/22.png)

---

## 11. Activity2 - Giải phương trình bậc hai

### 11.1 Thiết kế giao diện

Activity2 được dùng để giải phương trình bậc hai theo dạng:

Người dùng nhập:

* Hệ số `a`
* Hệ số `b`
* Hệ số `c`

sau đó nhấn nút:

```text id="c05zv4"
GIẢI
```

Ứng dụng sẽ tính toán và hiển thị kết quả.

Giao diện được xây dựng bằng:

* `EditText` – nhập dữ liệu.
* `Button` – thực hiện phép tính.
* `TextView` – hiển thị kết quả.

![Ảnh 23](images/23.png)

---

### 11.2 Xử lý logic giải phương trình

Sau khi người dùng nhập dữ liệu và nhấn nút giải, chương trình thực hiện:

### Bước 1: Lấy dữ liệu

```java id="fxnhdp"
Double.parseDouble()
```

để chuyển dữ liệu từ chuỗi sang số thực.

### Bước 2: Tính Delta

\Delta=b^2-4ac

### Bước 3: Kiểm tra điều kiện

**TH1:** Δ < 0

→ phương trình vô nghiệm.

**TH2:** Δ = 0

→ phương trình có nghiệm kép.

x=\frac{-b}{2a}

**TH3:** Δ > 0

→ phương trình có hai nghiệm phân biệt.

x_1=\frac{-b+\sqrt{\Delta}}{2a}

x_2=\frac{-b-\sqrt{\Delta}}{2a}

Sau khi tính xong, kết quả sẽ hiển thị ra `TextView`.

![Ảnh 24](images/24.png)

---

### 11.3 Kết quả hoạt động

Khi nhập:

```text id="jlwm4h"
a = 1
b = 3
c = 2
```

Ứng dụng hiển thị:

```text id="jzjlwm"
x1 = -1
x2 = -2
```

Điều này cho thấy chức năng xử lý phương trình bậc hai hoạt động chính xác.

Ngoài ra, sau khi giải xong bài toán, ứng dụng còn thực hiện gửi dữ liệu lên API của hệ thống theo yêu cầu đề bài.

Dữ liệu gửi bao gồm:

* mã sinh viên
* input
* output

Giúp ghi nhận kết quả xử lý từ ứng dụng.

![Ảnh 25](images/25.png)

---

## 12. Activity3 - WebView

### 12.1 Giới thiệu

Activity3 được xây dựng nhằm hiển thị website trực tiếp trong ứng dụng bằng thành phần **WebView**.

WebView cho phép ứng dụng Android hiển thị nội dung website giống như một trình duyệt mini.

Địa chỉ website sử dụng:

```text id="0lq58s"
https://k58kmt.tdh.io.vn?masv=K225480106016
```

Để sử dụng WebView, ứng dụng cần khai báo quyền:

```xml id="1e1h8v"
android.permission.INTERNET
```

trong file `AndroidManifest.xml`.

![Ảnh 26](images/26.png)

---

### 12.2 Xử lý WebView bằng Java

Trong Java, em tiến hành ánh xạ:

```java id="mhn0ku"
WebView webView;
```

Sau đó cấu hình:

```java id="n20sk1"
webView.getSettings()
.setJavaScriptEnabled(true);
```

Giúp website hoạt động đầy đủ hơn.

Tiếp theo:

```java id="kmh4eu"
webView.setWebViewClient(
new WebViewClient()
);
```

Mục đích:

Không mở trình duyệt ngoài mà hiển thị website ngay bên trong ứng dụng.

Cuối cùng:

```java id="x44pql"
webView.loadUrl()
```

được sử dụng để tải website.

Kết quả ứng dụng hiển thị đúng thông tin theo mã sinh viên:

```text id="klt3q2"
K225480106016
```

bao gồm:

* Họ tên.
* Ngày sinh.
* Số điện thoại.
* Bộ đếm truy cập.

![Ảnh 27](images/27.png)

---

# KẾT LUẬN

Qua bài tập lớn môn **Phát triển ứng dụng trên thiết bị di động - TEE0419**, em đã tìm hiểu và thực hành được nhiều kiến thức quan trọng trong phát triển ứng dụng Android.

Các kiến thức đã học gồm:

* MIT App Inventor.
* Block Programming.
* Thiết kế giao diện kéo thả.
* Android Studio.
* Java Language.
* AndroidManifest.xml.
* Activity Lifecycle.
* XML Layout.
* Event xử lý Button.
* Intent chuyển màn hình.
* WebView.
* JSON.
* Assets.
* ListView và Spinner.
* Xử lý dữ liệu offline.
* API JSON.

Thông qua bài tập, em hiểu rõ hơn quy trình phát triển ứng dụng Android từ thiết kế giao diện đến xử lý logic và hiển thị dữ liệu thực tế.

Đồng thời, bài tập cũng giúp em nâng cao kỹ năng lập trình Java, tư duy xử lý dữ liệu và xây dựng ứng dụng Android có tính ứng dụng thực tế.
