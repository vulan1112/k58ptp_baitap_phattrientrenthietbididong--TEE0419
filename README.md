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
2. Viết app sử dụng Android Studio
   + Android manifest.xml  => mô tả gì? app cần quyền để do-st: khai báo ntn? để làm gì?
   + vòng đời của 1 ứng dụng android.
     code tự sinh sau khi tạo 1 project: có sẵn hàm onCreate: tại sao???
   + Code: java language. 
     app cần check xem có quyền để do-st? : code ntn? ý nghĩa?
     giao diện: (res/layout) mô tả bằng file XML + UI Design review
        + thuộc tính text, hoặc các thuộc tính khác: giá trị hardcode => lưu vào nới khác, tham chiếu tới nó:
          cú pháp của việc tham chiếu là gì?
          ưu điểm của việc tham chiếu này?
          OS hỗ trợ auto việc lấy giá trị tham chiếu theo LOCATION, LANGUAGE, THEME
          việc hỗ trợ auto này giúp app làm được điều gì?	
        + đối tượng chứa: gộp các đối tượng con lại: cùng 1 quy luật sắp xếp để hiển thị 
          các đối tượng con nằm kề nhau theo chiều dọc | hoặc ngang, gravity
     code tương tác với layout: vd hiển thị text
          mong muốn text hiển thị phù hợp với thiết lập LOCATION, LANGUAGE, THEME của người dùng
          thì làm ntn? (tránh hardcode)
     event (sự kiện) người dùng tác động vào app: CLICK vào button, click vào text,...
          với 1 sự kiện nào đó, muốn chạy 1 đoạn code để do-st
          thì LAYTOUT cần làm gì?
              CODE viết như nào (2 cách)
---------------------------
   trong app có các thư mục đặc biệt: Assets
     khi sử dụng Window Explorer để copy các files + folder vào trong Assets
     thì khi compiler: mọi file này đều đi theo app, nằm trong app
     trong app có thể truy cập được đến các file này
     cú pháp truy cập vào là gì?
     lợi ích của việc app có sẵn các files (offline cũng có)?
     ứng dụng: app hướng dẫn việc X

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

Giao diện Preview


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

==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets
         format dữ liệu: tuỳ ý, nội dung tuỳ ý
         công cụ để hiển thị dữ liệu: tuỳ ý
         có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý.
         SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ
         MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ
                    DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN)
                    DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU.
                    (ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN)
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
=======================
    vết để lại: mô tả quá trình làm bài tập ra file .md => upload github
    kèm hình ảnh minh hoạ quá trình làm.

    print ra giấy đóng quyển, nộp bm.

