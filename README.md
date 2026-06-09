# k58ptp_baitap_phattrientrenthietbididong--TEE0419
## VU LAN_K225480106036_PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419
### BÀI TẬP LỚN:
# I. Viết phần mềm trên công cụ Mit App inventor
   (tập trung vào quy trình tạo ra phần mềm)
   app có 3 screen:
   + about về bản thân+nút gọi sang 2 screen còn lại
   + giải 1 bài toán đơn giản
   + sử dụng webview: hiển thị 1 trang web có sẵn, hỗ trợ giao diện điện thoại
# mô tả: thanh công cụ có gì? kéo thả + thay đổi thuộc tính: làm ntn, để làm gì?
1. block: mô tả bản chất việc kéo thả block ntn?
2. ưu điểm gì so với viết code? nhược điểm?
3. copy paste block ? (backpack)

Bước đầu đăng nhập:

<img width="975" height="547" alt="image" src="https://github.com/user-attachments/assets/3db02786-9e0b-4589-8024-96652fd3321a" />

Đăng nhập xong:

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/ad1e06c3-a7c6-401e-a04f-e22bce66e595" />

Bắt đầu tạo:

Thông tin bản thân

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/0890cbc7-1e3d-4a1e-a3d7-b6d270780222" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/ca7277f4-149c-4e8e-b0cd-0f525c141144" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/bbe849ba-7ab8-466d-9a65-4ee4c1b96d7f" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/01244284-5486-4fdc-8ef4-7f041f2472e8" />

Gắn URL vào ScreenWeb

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/d7674ae9-4bd9-491e-895d-83af54b42c3e" />

Cách thiết lập URL cho WebViewer

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/77d43c72-1ab6-4e0f-8a22-95e40a0003df" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/92d0cb53-5f4d-4848-a5b7-48c5626f9f02" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/432fb80d-1d1e-42e9-bba8-25b165dcef5f" />

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/42ffe7b8-6c84-4166-9c56-e4637457ea60" />

Thiết kế giao diện ScreenToan (Designer)

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/8e9e6857-8eb3-47a0-984e-87893a100958" />

Lập trình logic (Blocks)

<img width="975" height="548" alt="image" src="https://github.com/user-attachments/assets/c7aad646-b6bb-4ea2-b27a-b06b05206107" />

Kết Quả cuối sau khi thêm "quay lại"

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8ee3be2d-9d8a-41c8-993a-6ca6238fb502" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/90ab0ef3-6a38-447d-acf5-24fa11e98863" />

<img width="1184" height="2560" alt="image" src="https://github.com/user-attachments/assets/78df8bd4-4a96-424e-bd05-be28f9af43e8" />

<img width="1184" height="2560" alt="image" src="https://github.com/user-attachments/assets/f1a08590-b788-4884-aa54-37ec2efcbb80" />

<img width="1184" height="2560" alt="image" src="https://github.com/user-attachments/assets/73342a5d-52e3-478c-a99f-edc2f1fcfba7" />

thay url bất kỳ hỗ trợ điện thoại

<img width="1812" height="1080" alt="image" src="https://github.com/user-attachments/assets/6b393326-6e2f-4e54-8559-fff0f89a0529" />

<img width="1184" height="2560" alt="image" src="https://github.com/user-attachments/assets/149a7f84-1bde-4c66-a49c-469c56ab096e" />

# 2. Viết app sử dụng Android Studio
## 1. AndroidManifest.xml dùng để làm gì?
  
`AndroidManifest.xml` là file cấu hình quan trọng của ứng dụng Android. File này dùng để khai báo thông tin chính của ứng dụng như tên app, các Activity, quyền truy cập, Activity chạy đầu tiên và một số cấu hình hệ thống.

Ví dụ:
<activity android:name=".MainActivity" />
<activity android:name=".ToanActivity" />
<activity android:name=".WebActivity" />

2. App cần quyền để làm gì? Khai báo quyền như thế nào?

Ứng dụng cần quyền để sử dụng một số chức năng của thiết bị hoặc hệ thống. Ví dụ app cần truy cập Internet để mở WebView hoặc gửi API thì phải khai báo quyền Internet.

Cách khai báo:

<uses-permission android:name="android.permission.INTERNET" />

Dòng này được đặt trong thẻ <manifest> và nằm ngoài thẻ <application>.
3. Quyền INTERNET dùng để làm gì?

Quyền INTERNET cho phép ứng dụng truy cập mạng. Trong bài này quyền Internet dùng để:

Mở website bằng WebView.
Gửi dữ liệu bài toán lên API.
Nhận phản hồi từ server.
4. Vòng đời của một Activity Android gồm những hàm nào?

Vòng đời của một Activity Android gồm các hàm chính:

onCreate()
onStart()
onResume()
onPause()
onStop()
onDestroy()

Trong đó:

onCreate() được gọi khi Activity được tạo lần đầu.
onStart() được gọi khi Activity bắt đầu hiển thị.
onResume() được gọi khi Activity sẵn sàng tương tác.
onPause() được gọi khi Activity tạm dừng.
onStop() được gọi khi Activity không còn hiển thị.
onDestroy() được gọi khi Activity bị đóng hoặc bị hủy.
5. Vì sao khi tạo project Android có sẵn hàm onCreate?

Khi tạo project Android, Android Studio tự sinh hàm onCreate() vì đây là hàm khởi tạo đầu tiên của Activity. Hàm này dùng để nạp giao diện, ánh xạ các thành phần giao diện và xử lý các thao tác ban đầu.

Ví dụ:

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
6. setContentView dùng để làm gì?

setContentView() dùng để gắn file giao diện XML với Activity Java.

Ví dụ:

setContentView(R.layout.activity_main);

Dòng này có nghĩa là Activity sẽ sử dụng giao diện được thiết kế trong file activity_main.xml.

7. Java được dùng để làm gì trong Android Studio?

Trong Android Studio, Java được dùng để viết logic xử lý cho ứng dụng. Ví dụ:

Xử lý sự kiện bấm nút.
Chuyển màn hình bằng Intent.
Tính toán dữ liệu.
Đọc file trong Assets.
Gửi API.
Mở WebView.
8. App cần kiểm tra quyền để làm gì?

App cần kiểm tra quyền để đảm bảo người dùng đã cấp quyền trước khi sử dụng các chức năng nhạy cảm như Camera, vị trí hoặc bộ nhớ.

Ví dụ kiểm tra quyền Camera:

if (checkSelfPermission(android.Manifest.permission.CAMERA)
        != PackageManager.PERMISSION_GRANTED) {
    requestPermissions(
            new String[]{android.Manifest.permission.CAMERA},
            100
    );
}

Ý nghĩa: nếu app chưa có quyền Camera thì app sẽ xin quyền từ người dùng.

9. Giao diện Android được đặt ở đâu?

Giao diện Android thường được đặt trong thư mục:

res/layout

Ví dụ:

activity_main.xml
activity_toan.xml
activity_web.xml

Mỗi file XML thường tương ứng với một màn hình trong app.

10. File XML trong res/layout dùng để làm gì?

File XML dùng để mô tả giao diện của ứng dụng. Trong XML có thể khai báo các thành phần như:

TextView
Button
EditText
WebView
LinearLayout
ScrollView

Ví dụ:

<Button
    android:id="@+id/btnToan"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:text="Mở màn hình giải toán" />
11. UI Design Review là gì?

Trả lời:

UI Design Review là phần xem trước giao diện trong Android Studio. Khi mở file XML, có thể chọn Design hoặc Split để xem giao diện ứng dụng hiển thị như thế nào trên điện thoại.

Phần này giúp kiểm tra bố cục, màu sắc, kích thước và vị trí các thành phần trước khi chạy app.

12. Hardcode là gì?

Hardcode là việc viết trực tiếp nội dung vào code hoặc file XML.

Ví dụ:

android:text="Mở màn hình giải toán"

Cách này chạy được nhưng không tốt nếu app cần hỗ trợ nhiều ngôn ngữ hoặc cần quản lý nội dung tập trung.

13. Cách tránh hardcode trong Android là gì?

Để tránh hardcode, nên lưu nội dung text vào file:

res/values/strings.xml

Ví dụ trong strings.xml:

<string name="open_toan">Mở màn hình giải toán</string>

Trong XML tham chiếu bằng:

android:text="@string/open_toan"
14. Cú pháp tham chiếu tài nguyên trong Android là gì?

Cú pháp tham chiếu tài nguyên trong XML là:

@loại_tài_nguyên/tên_tài_nguyên

Ví dụ:

android:text="@string/app_name"

Trong Java có thể lấy bằng:

getString(R.string.app_name);
15. Ưu điểm của việc tham chiếu tài nguyên là gì?

Việc tham chiếu tài nguyên có các ưu điểm:

Dễ quản lý nội dung.
Dễ chỉnh sửa.
Tránh lặp lại text nhiều lần.
Hỗ trợ đa ngôn ngữ.
Hỗ trợ theme sáng/tối.
Giúp app chuyên nghiệp hơn.
16. Android hỗ trợ tự động theo LOCATION, LANGUAGE, THEME như thế nào?

Android có thể tự động lấy tài nguyên phù hợp theo ngôn ngữ, khu vực và giao diện người dùng.

Ví dụ:

res/values/strings.xml
res/values-en/strings.xml

Nếu máy dùng tiếng Việt thì app lấy nội dung trong values. Nếu máy dùng tiếng Anh thì app có thể lấy nội dung trong values-en.

Điều này giúp app dễ hỗ trợ nhiều ngôn ngữ và nhiều nhóm người dùng khác nhau.

17. Đối tượng chứa trong Android là gì?

Đối tượng chứa là layout dùng để chứa các thành phần con và sắp xếp chúng theo một quy luật nhất định.

Ví dụ:

<LinearLayout>
    <TextView />
    <Button />
</LinearLayout>
18. LinearLayout dùng để làm gì?

LinearLayout dùng để sắp xếp các thành phần con theo chiều dọc hoặc chiều ngang.

Sắp xếp theo chiều dọc:

android:orientation="vertical"

Sắp xếp theo chiều ngang:

android:orientation="horizontal"
19. Gravity dùng để làm gì?

gravity dùng để căn chỉnh nội dung bên trong layout hoặc bên trong một thành phần giao diện.

Ví dụ căn giữa theo chiều ngang:

android:gravity="center_horizontal"
20. Code Java tương tác với layout như thế nào?

Muốn Java tương tác với layout, cần đặt id cho đối tượng trong XML, sau đó dùng findViewById() để ánh xạ sang Java.

Ví dụ XML:

<TextView
    android:id="@+id/txtKq"
    android:layout_width="match_parent"
    android:layout_height="wrap_content" />

TextView txtKq = findViewById(R.id.txtKq);
txtKq.setText("Kết quả");

21. Muốn text phù hợp với ngôn ngữ người dùng thì làm thế nào?

Không nên viết text trực tiếp trong Java hoặc XML. Nên lưu text trong strings.xml, sau đó tham chiếu bằng @string/....

Ví dụ:

android:text="@string/ket_qua"

Trong Java:

txtKq.setText(getString(R.string.ket_qua));

Nhờ vậy Android có thể tự chọn text phù hợp theo ngôn ngữ của thiết bị.

22. Event trong Android là gì?

Event là sự kiện xảy ra khi người dùng tác động vào ứng dụng, ví dụ:

Click vào Button.
Click vào TextView.
Nhập dữ liệu vào EditText.
Chọn một mục trong danh sách.
23. Layout cần làm gì để code xử lý event?

Layout cần đặt id cho đối tượng cần xử lý sự kiện.

Ví dụ:

<Button
    android:id="@+id/btnTinh"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:text="Tính tổng" />

Sau đó trong Java dùng:

Button btnTinh = findViewById(R.id.btnTinh);
24. Code xử lý sự kiện click viết như thế nào? Cách 1

Cách 1 là dùng lambda:

btnTinh.setOnClickListener(v -> {
    txtKq.setText("Đã bấm nút tính");
});

Cách này ngắn gọn, dễ đọc và được sử dụng trong bài thực hành.

25. Code xử lý sự kiện click viết như thế nào? Cách 2

Cách 2 là dùng View.OnClickListener:

btnTinh.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        txtKq.setText("Đã bấm nút tính");
    }
});

Cách này dài hơn nhưng dễ hiểu với người mới học vì thể hiện rõ hàm onClick.

26. Assets trong Android là gì?

Assets là thư mục đặc biệt dùng để lưu các file dữ liệu đi kèm với ứng dụng. Các file này có thể là:

.txt
.html
.json
ảnh
âm thanh
dữ liệu offline
27. Khi copy file vào Assets thì chuyện gì xảy ra?

Khi copy file vào thư mục assets, các file này sẽ được đóng gói cùng ứng dụng khi biên dịch. Khi cài app lên điện thoại, file vẫn nằm trong app và có thể được truy cập bằng code.

28. Cú pháp đọc file trong Assets là gì?

Cú pháp đọc file trong Assets:

InputStream inputStream = getAssets().open("dan_toc_viet_nam.txt");

Sau đó có thể dùng BufferedReader để đọc từng dòng:

BufferedReader reader = new BufferedReader(
        new InputStreamReader(inputStream)
);
29. Lợi ích của việc app có sẵn file trong Assets là gì?

Lợi ích của Assets là:

App có thể hoạt động offline.
Không phụ thuộc Internet.
Dữ liệu đi kèm app.
Tốc độ đọc nhanh.
Phù hợp với app hướng dẫn, tài liệu học tập, từ điển nhỏ.
30. Ứng dụng Assets trong bài là gì?

Trong bài, em xây dựng ứng dụng đọc dữ liệu offline từ Assets. App có hai mục nội dung:

Đặc điểm dân tộc Việt Nam
Chủ quyền biển đảo Việt Nam

Mỗi mục được lưu trong một file .txt riêng trong thư mục assets.

31. Dữ liệu trong Assets có đặc thù gì?

Dữ liệu trong bài là dữ liệu văn bản nhiều dòng, có tiêu đề, các ý chính và phần kết luận. Dữ liệu không cần xử lý phức tạp mà chỉ cần đọc và hiển thị.

32. Dùng thuật toán nào để xử lý dữ liệu Assets?

Thuật toán xử lý là đọc tuần tự từng dòng trong file bằng BufferedReader, sau đó dùng StringBuilder để ghép các dòng lại thành một chuỗi hoàn chỉnh.

Quy trình:

Mở file trong Assets
Đọc từng dòng
Ghép nội dung bằng StringBuilder
Hiển thị lên TextView
33. Dùng đối tượng nào để hiển thị dữ liệu Assets?

Dữ liệu được hiển thị bằng TextView. Vì nội dung dài nên đặt TextView bên trong ScrollView để người dùng có thể cuộn xem toàn bộ nội dung.

Ví dụ:

<ScrollView>
    <TextView
        android:id="@+id/txtNoiDung" />
</ScrollView>
34. Kết quả đạt được của app Android Studio là gì?

Sau khi hoàn thành, ứng dụng có các chức năng:

Hiển thị màn hình giới thiệu sinh viên.
Chuyển sang màn hình giải toán.
Tính tổng hai số.
Gửi dữ liệu bài toán lên API.
Mở WebView hiển thị website.
Đọc dữ liệu offline từ thư mục Assets.
Hiển thị nội dung bằng TextView và ScrollView.
==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets
format dữ liệu: tuỳ ý, nội dung tuỳ ý
         
   công cụ để hiển thị dữ liệu: tuỳ ý
         có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý.
         SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ
         MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ
                    DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN)
                    DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU.
                    (ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN)

<img width="1920" height="1061" alt="image" src="https://github.com/user-attachments/assets/1cafb4f3-fc61-4d64-8b33-ee57bd74876d" />

<img width="1912" height="1079" alt="image" src="https://github.com/user-attachments/assets/7aaa2b85-2af0-44f0-a0db-8a75fb401699" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4b05f3c9-a2e5-410f-9ea6-5d90b93d0567" />

<img width="1919" height="1080" alt="image" src="https://github.com/user-attachments/assets/302c8777-9ca2-45bd-a185-53bf0280a265" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9dd69aba-f0ba-4a80-b098-ed17150977f6" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/93ddf25b-0ff9-4c67-9c0c-61847b6842dd" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b090eb68-5caf-4e31-94db-70e8a9e563e5" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8bb72493-17a2-4a00-a745-c2866fb6be58" />

<img width="1915" height="1066" alt="image" src="https://github.com/user-attachments/assets/e5d57115-6ab1-4b12-8e96-340ce3e81b85" />

<img width="1912" height="1073" alt="image" src="https://github.com/user-attachments/assets/361ea7fa-db66-416f-aa3e-14f2aeb7ccd7" />

<img width="720" height="1520" alt="l5" src="https://github.com/user-attachments/assets/ebb69dbb-8370-4f22-83be-55723280a9d0" />

<img width="720" height="1520" alt="l2" src="https://github.com/user-attachments/assets/45dfaff9-4e15-4aee-b460-d4e0b7c81ae7" />

<img width="720" height="1520" alt="l4" src="https://github.com/user-attachments/assets/0315c0b0-7a95-407c-b837-be1dc980bc86" />

------------------------
APP2 (android studio):  tạo app tương đương với Mit App inventor
  app có 3 activity
  + activity1: about: about+nút gọi sang 2 activity còn lại
  + activity2: giải toán đơn giản (tuỳ ý). mỗi khi giải xong bài toán: gọi api tại https://k58kmt.tdh.io.vn/api
    để gửi bài toán lên đó
    {app_by:mã số sv, input: {a:1,b:2,c:3,name:"hello tắc kè"},output:{ketluan:"vô nghiệm", abc:"xyz", nghiem:3.14}}
    nhận lại json: {ok:1, stt:1234}
  + activity3: 
    dùng web-view để truy cập từ 
    1 trang web https://k58kmt.tdh.io.vn?masv=mã sv của bạn

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c9f314ef-5022-4018-9304-09c7697dd03c" />

Setup SDK: chọn "Eclipse Temurin 17.0.18"

<img width="840" height="354" alt="image" src="https://github.com/user-attachments/assets/31424424-2409-484b-92e5-433b4e0275b5" />

**1. Build project cho cho Android Studio hết lỗi trước**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5ce9c187-8e59-4278-b2ca-62e99bbb9177" />

<img width="1918" height="1080" alt="image" src="https://github.com/user-attachments/assets/189c4fb4-069c-4998-bfaf-73f1c7364f85" />

**2. Code giao diện**

TextView

Button mở màn hình giải toán

Button mở WebView

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9420260a-ee59-4118-b0e6-b7e487737e67" />

**3. Tạo Activity**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/70e345c7-377e-4f6e-8f1a-8c20afba8bea" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/559baef6-4a40-431a-a428-54db77674a80" />

Cây thư mục có:

1.MainActivity

2.ToanActivity

3.WebActivity

<img width="1920" height="1072" alt="image" src="https://github.com/user-attachments/assets/fded4552-4e6d-4408-9337-1a81889366f2" />

AndroidManifest

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0b3995cb-d30d-482a-8486-daf3560d5aa4" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/66b4aeb2-be7f-45e7-831c-9f34df756f8e" />

Code Java

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/350dddf3-039f-4c89-a360-ac52315ad2c7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/bbe8f95f-56b0-40b4-92dd-d28ad930dd0d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0e3ff156-e0d6-4596-9f03-420b5ced5b65" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9985e9f7-8425-4f44-8312-4dfe09af785d" />

Gửi API

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8fb6e200-1757-4471-ab79-adaae8294ef0" />

Nhấn nút Run ▶ Trong Android Studio

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ee0de941-0515-408f-b15e-4f0f28349566" />

Chạy app trên điện thoại

<img width="720" height="1520" alt="trang lan1" src="https://github.com/user-attachments/assets/04b6902b-16eb-452d-9b59-8d6f3a38126c" />

<img width="720" height="1520" alt="trang lan2" src="https://github.com/user-attachments/assets/c70d2de9-3cf1-4dce-b7f2-3b5f3ce6461b" />

<img width="720" height="1520" alt="trang lan2 1" src="https://github.com/user-attachments/assets/5321b332-bd1b-4b08-9cf9-8720fb2f5811" />

<img width="720" height="1520" alt="trang lan3" src="https://github.com/user-attachments/assets/8d6d3e91-22a9-4093-9ed8-7d7f524ec965" />

TEST API

<img width="720" height="1520" alt="t1" src="https://github.com/user-attachments/assets/6f04b0d4-40f0-491e-95bf-df73483734be" />

Minh chứng app trên điện thoại android

<img width="720" height="1520" alt="l1" src="https://github.com/user-attachments/assets/8dc58f52-6993-4f3f-9ee3-30b01a3ca90b" />

=======================
    vết để lại: mô tả quá trình làm bài tập ra file .md => upload github
    kèm hình ảnh minh hoạ quá trình làm.

    print ra giấy đóng quyển, nộp bm.

