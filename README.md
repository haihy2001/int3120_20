# Mobile Homework

<!-- TABLE OF CONTENTS -->
<!-- <details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#week-1">Week 1</a>
      <ul>
        <li><a href="#lesson-1">Lesson 1</a></li>
        <li><a href="#lesson-2">Lesson 2</a></li>
        <li><a href="#lesson-3">Lesson 3</a></li>
        <li><a href="#lesson-3">Lesson 4</a></li>
        <li><a href="#lesson-3">Lesson 5</a></li>
        <li><a href="#lesson-3">Lesson 6</a></li>
      </ul>
      <a href="#week-1">Week 2</a>
      <ul>
        <li><a href="#lesson-7">Lesson 7</a></li>
        <li><a href="#lesson-8">Lesson 8</a></li>
        <li><a href="#lesson-9">Lesson 9</a></li>
        <li><a href="#lesson-10">Lesson 10</a></li>
      </ul>
    </li>
  </ol>
</details> -->

## Week 1
#### Lesson 1
- Giới thiệu các tính năng, điểm mạnh của Flutter.
#### Lesson 2
- Cài đặt Flutter và môi trường phát triển.
![Kiểm tra môi trường phát triển](imgs/flutter-doctor.png)
#### Lesson 3
- Ứng dụng Hello World:
  ![Bài 3](/imgs/bai3.png)
#### Lesson 4
- Mọi thứ trong Flutter đều là widget, widget là thành giao diện cơ bản nhất tạo nên toàn bộ giao diện của ứng dụng.
- Các tính năng tương tác sẽ đước tích hợp bất cứ khi nào nhờ GestureDetector widget.
- Trạng thái của các widget được quản lý cập nhật bởi StatefulWidget widget.
- Flutter cung cấp thiết kế class để bất kỳ lớp nào có thể được lập trình tùy thuộc vào độ phức tạp của tác vụ.
#### Lesson 5
- Dart là một ngôn ngữ lập trình mã nguồn mở, đa năng và được phát triển bởi Google.
- Là ngôn ngữ lập trình hướng đối tượng và sử dụng cú phát của C (C-style syntax)
#### Lesson 6
- Trong Flutter, widget được phân loại dựa trên chức năng thành 4 nhóm:
  - Platform widgets: Các widget giao diện đặc thù theo từng nền tảng.
  - Layout widgets: Các widget hỗ trợ bố trí giao diện
  - State maintenance widgets: Các widget quản lý trạng thái
  - Platform independent / basic widgets: Các widget cơ bản độc lập với nền tảng
- Demo:
  ![Bài 6](/imgs/bai6.png)
## Week 2
#### Lesson 7
- Có hai loại widget layout chính:
  - Single Child Widgets - Chỉ có một widget con
  - Multiple Child Widgets - Có nhiều widget con
- Demo:
  ![Bài 7](/imgs/bai7.png)
#### Lesson 8
- Hỗ trợ một số cử chỉ: Tap, Double Tap, Drag, Flick, Pinch, Spread/Zoom, Panning
- Flutter cung cấp widget GestureDetector để xử lý tất cả các cử chỉ.
- Flutter cũng cung cấp một cơ chế phát hiện cử chỉ cấp thấp thông qua Listener widget
- Flutter còn cung cấp một số nhỏ các widget để thực hiện các cử chỉ cụ thể đơn giản cũng như phức tạp
- Demo:
  ![Bài 8](/imgs/bai8.png)
#### Lesson 9
- Quản lý sate (trạng thái) của ứng dụng là một trong những bước quan trọng và cần thiết trong vòng đời của một ứng dụng.
- Việc quản lý trạng thái có thể chia làm hai loại:
  - Ephemeral (ngắn hạn): Kéo dài trong thời gian ngắn. Flutter hỗ trợ quản lý trạng thái loại này thông qua StatefulWidget.
  - App state (trạng thái ứng dụng): Kèo dài trong toàn bộ ứng dụng. Flutter hỗ trợ quản lý trạng thái loại này thông qua scoped_model
#### Lesson 10
- Widget được kết thừa từ Statefulwidget để duy trì trạng thái và quản lý các trạng thái con của nó.
- Demo ứng dụng sử dụng Statefulwidget để làm RatingBox:
  ![Bài 10](/imgs/bai10.png)
#### Lesson 11
- Flutter cung cấp một phương pháp đơn giản để quản lý trạng thái của ứng dụng sử dụng scoped_model package. Nó cung cấp 3 class chính:
  - Model: Model đóng gói trạng thái của một ứng dụng. Model có một phương thức duy nhất là notifyListeners, nó được gọi bất cứ khi nào trạng thái của Model thay đổi. notifyListeners sẽ thực hiện các công việc cần thiết để cập nhật giao diện.
  - ScopedModel: ScopedModel là một widget để dễ dàng chuyển Data Model từ widget cha xuống con, cháu và rebuild lại các widget con giữ các model khi model này cập nhật.
  - ScopedModelDescendant: là một widget lấy Data Model từ cha và build lại UI khi Data Model thay đổi.
- Sử dụng scoped_model để thay cho StatefulWidget để làm RatingBox:
  ![Bài 11](/imgs/bai11.png)
#### Lesson 12
- Flutter cung cấp cho chúng ta lớp Routing cơ bản - MaterialPageRoute với hai phương thức - Navigator.push và Navigator.pop
  - MaterialPageRoute: một widget được sử dụng để render giao diện người dùng nhằm thay thế toàn bộ màn hình với một hiệu ứng chuyển đặc biệt nào đó
  - Navigation.push: Giúp ta chuyển sang một màn hình khác
  - Navigation.pop: Được sử dụng để quay về trang trước
- Ứng dụng áp dụng routing để chuyển sang màn hình chi tiết của Product khi bấm vào Product đó:
  ![Bài 12](/imgs/bai12.png)
## Week 3
#### Lesson 13
- Flutter animation dựa trên các đối tượng animation. Lõi của các lớp animation nó hoạt động như sau:
  - Animation:
    - Tạo ra giá trị và được thêm vào giữa hai số (bắt đầu và kết thúc animation). Các kiểu animation thường được sử dụng là: Animation, Animation, Animation
    - AnimationController: đối tượng animation đặc biệt dùng để điều khiển các hiệu ứng của chính nó. Nó tạo ra các giá trị mới bất cứ khi nào ứng dụng sẵn sàng cho một frame mới, hỗ trợ các animation tuyến tính
  - CurvedAnimation: cơ bản giống như AnimationController nhưng hỗ trợ animation phi tuyến tính
  - Tween: kế thừa từ Animatable và tạo các giá trị bất kì khác 0 và 1. Nó được sử dụng cùng với đối tượng animation bởi phương thức animate()
- Demo

#### Lesson 14
- Flutter cung cấp framework chung để truy cập vào các nền tảng có tính năng riêng biệt thông qua giao thức đơn giản là messaging. Client (Flutter code), mã nền tảng và Host liên kết với một thông báo chung gọi là Message Channel
- Demo:
  ![Bài 14](/imgs/bai14.png)
  ![Bài 14](/imgs/bai14_2.png)
#### Lesson 16
- Dart Package là một thư viện hay mô hình đơn giản có thể chia sẻ. Về cơ bản, Dart Package tương tự Dart Application, tuy nhiên nó không truy cập vào các điểm chính của ứng dụng
- Các kiểu package:
  - Dart package: có thể sử dụng trên nhiều môi trường
  - Flutter package: phụ thuộc vào Flutter framework, có thể chỉ sử dụng trong môi trường mobile
  - Flutter plugin: phụ thuộc vào Flutter framework và cả nền tảng (iOS SDK hay Android SDK)
- Demo:
  ![Bài 16](/imgs/bai16_1.png)
  ![Bài 16](/imgs/bai16_2.png)
#### Lesson 17
- Flutter cung cấp package http, http là một thư viện Future-based sử dụng await và async. Nó cung cấp phương thức cấp cao và đơn giản để phát triển REST
  - Lớp http cung cấp chức năng để làm việc với tất cả các kiểu dữ liệu HTTP được request
  - Phương thức http có sử dụng url, và bổ sung thông tin thông qua Dart Map
- Một vài phương thức chính:
  - read: gửi yêu cầu sử dụng phương thức GET và trả về Future
  - get: gửi yêu cầu sử dụng phương thức GET và trả về Future. Response là lớp giữ lại các thông tin phản hồi
  - post: gửi yêu cầu sử dụng phương thức POST, đưa giá trị lên sever và phản hồi Future
  - put: gửi yêu cầu sử dụng phương thức PUT và trả về phản hồi Future
  - head: gửi yêu cầu sử dụng phương thức HEAD và trả về phản hồi Future
  - delete: gửi yêu cầu sử dụng phương thức DELETE và trả về phản hồi Future
- Demo:
  ![Bài 17](/imgs/bai17.png)
  ![Bài 17](/imgs/bai17_2.png)
#### Lesson 19
- Hiện nay, các ứng dụng có thể được sử dụng từ nhiều nơi trên thế giới, vì thế các ứng dụng phải hiển thị nội dung phù hợp với ngôn ngữ của quốc gia đó
- Flutter hỗ trợ ứng dụng làm việc với đa ngôn ngữ (Internationalizing). Trong đó, có thể kể đến 3 lớp localization:
  - Locale: lớp được sử dụng để nhận diện ngôn ngữ người sử dụng
  - Localizations: widget chung được sử dụng để set Locale và nguồn localized của lớp con
  - LocalizationsDelegate: lớp factory thông qua widget Localizations được tải. Nó có 3 phương thức overridable như sau:
    - isSupported: Chấp nhận một biến kiểu Locale và kiểm tra locale đó có được hỗ trợ không
    - load: Chấp nhận ngôn ngữ được chọn và tải dữ liệu tương ứng ngôn ngữ đó
    - shouldReload: Liệu có nên tải lại khi widget Localizations được rebuild
- Demo:
  ![Bài 19](/imgs/bai19_1.png)
  ![Bài 19](/imgs/bai19_2.png)
  ![Bài 19](/imgs/bai19_3.png)
  ![Bài 19](/imgs/bai19_4.png)