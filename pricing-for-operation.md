# Báo giá, Quy trình và Vận hành ứng dụng Web trên vercel

Với template Finbiz, mình lấy giá trọn gói thiết kế và triển khai ứng dụng là 6.500.000 VND.

## I. Quy trình

Quy trình từ bắt đầu tới lúc bàn giao như sau:

### 1. File thiết kế trên Figma:

- File thiết kế trên Figma được triển khai khoảng 1 tuần với đầy đủ các trang trên ứng dụng Web với giao diện trên Desktop (không bao gồm responsive đến các ứng dụng trên thiết bị nhỏ hơn như Tablet và Mobile, các giao diện này sẽ được mình tự responsive phù hợp khi viết code).

- Bàn giao file thiết kế và chỉnh sửa tuỳ ý khách, nhanh hay chậm tuỳ vào chỉnh sửa nhiều hay ít.

### 2. Viết code bằng Next.js theo file thiết kế sẵn:

- Mình thường làm vào buổi tối tầm 2 - 3 tiếng/ ngày nên thời gian sẽ tuỳ dự án. Dự đoán dự án này tầm 1 tháng (bao gồm luôn thời gian fix bug phát sinh).

- Lúc này mình vừa viết code vừa chạy trên web demo, khách có thể theo dõi web bằng link mình đưa (link có dạng đuôi .vercel.app)

### 3. Chạy demo bàn giao trên host của mình:

- Chạy demo đầy đủ tính năng trên host của mình. Khách chưa ưng ý tính năng nào thì mình fix lại, tất nhiên là thời gian phụ thuộc vào khách muốn sửa nhiều hay ít.

- Lúc này, khách thanh toán trước 50% (3.250.000 VND) sau khi sửa các tính năng xong.

### 4. Chạy trên host thực tế:

- Khách đăng ký tài khoản Vercel giúp mình. Đưa mình mật khẩu và email tài khoản đăng ký để mình triển khai trên tài khoản Vercel của khách.

- Chi phí vận hành web tuỳ vào nhu cầu và lượng người dùng trang web. (Xem phần II)

- Sữa lỗi triển khai trên web liên tục nếu có đến khi bàn giao.

### 5. Bàn giao website và Thanh toán:

- Nếu không còn vấn đề gì thì thanh toán 50% còn lại. (3.250.000 VND)

## II. Chi phí vận hành:

### 3. Chi phí mua domain:

- Domain là địa chỉ website (như facebook.com, x.com, ...) phải được mua từ bên thứ 3, sau đó cung cấp một số thông tin cho mình để mình trỏ tới địa chỉ đó từ Vercel. Domain nên được mua từ 2 năm trở lên để tránh bị claim bởi người khác.

- Giá của một domain tuỳ thuộc vào nhiều yếu tố (đuôi, tên domain, đã bị sở hữu bởi người khác chưa), cái này tuỳ khách quyết định. Mình chỉ cần thông tin sau khi mua.

- Tham khảo giá domain trên website: [www.godaddy.com](https://www.godaddy.com/vi-vn)

### 2. Chi phí vận hành trên Vercel:

- Vì ứng dụng chạy trên host thuộc tài khoản Vercel của khách nên toàn bộ chi phí hàng tháng khách tự kiểm soát theo nhu cầu của mình.

- Chi phí hàng tháng là miễn phí đối với Hobby Plan (mặc định khi đăng ký tài khoản Vercel). Hobby Plan của Vercel phù hợp cho công ty nhỏ hoặc startup ít người dùng và giới hạn traffic.

- Ứng dụng web sử dụng Hobby Plan sẽ chia sẻ chung CPU và RAM. Đôi khi sẽ bị sleep (nếu vào lại sẽ lâu hơn bình thường một chút) nếu không có người dùng vào web trong một khoảng thời gian nhất định (theo mình biết là một tuần).

- Nếu traffic của ứng dụng vượt quá giới hạn của Hobby Plan, ứng dụng sẽ bị pause không thể truy cập. Khách cần phải nâng lên Pro Plan của Vercel với giá 20$/tháng. Yên tâm là với ứng dụng của ông thì mình nghĩ chưa vượt quá Hobby Plan vì lượng người dùng phải lên đến hàng trăm nghìn lượt truy cập mỗi tháng mới cần tới Pro Plan.

- Xem so sánh Hobby Plan với Pro Plan tại link sau: [Vercel Pricing](https://vercel.com/pricing)

### 3. Chi phí hỗ trợ/thêm tính năng:

- Với chỉnh sửa đơn giản (sửa văn bản trên web, sửa một số tính năng đã có, ...) hoặc lỗi phát sinh lúc vận hành từ phía mình, mình sẽ thực hiện hoặc sửa lỗi mà không lấy thêm chi phí trong vòng 1 năm kể từ lúc bàn giao.

- Với việc thêm tính năng (xác thực người dùng, thanh toán, ...), mình sẽ lấy phí theo thoả thuận. Nếu khách thấy không hợp lý, mình sẽ bàn giao toàn bộ source code trên Github cho khách thuê bên thứ 3 thêm tính năng và hỗ trợ support cho bên thứ 3 qua email.

## III. Vận hành:

### 1. Quản lý yêu cầu tư vấn của khách hàng:

- Mình sẽ tạo một trang admin và tài khoản admin (mật khẩu có thể thay đổi được) để bên công ty truy cập vào quản lý các yêu cầu tư vấn phía khách hàng. Mỗi khi khách hàng điền form Book, sẽ có email mới gửi vào trong inbox của công ty để thông báo, đồng thời cũng xuất hiện trên trang quản lý.

### 2. Quản lý bài viết blog trên Notion:

- Tính năng blog được lấy database từ Notion API nên khách hoàn toàn có thể viết blog trên Notion một cách bình thường. Các bài viết tự động xuất hiện trên website.