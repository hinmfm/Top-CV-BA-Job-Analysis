# Top-CV-BA-Job-Analysis
Dự án phân tích dữ liệu với dữ liệu được cào về từ Top CV nhằm phân tích tình hình thị trường công việc BA tại Hà Nội.
Dự án gồm các mục sau: 
1. [Mục đích phân tích](#Mục-đích-phân-tích) 
2. [Thu thập dữ liệu](#Thu-thập=dữ-liệu)
3. [Xử lý & làm sạch dữ liệu](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/processing-with-python)
4. [Phân tích dữ liệu](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product)
5. [Kể chuyện qua dữ liệu](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product/infographics%20%26%20powerbi)

Trong file README.md này sẽ là giải thích thứ tự file nên đọc theo và giải thích tổng quan về mỗi file sẽ bao gồm những gì. File cũng sẽ có một danh mục nội dung phía dưới đây để phục vụ cho việc tra cứu.
## Danh mục nội dung
- [Mục đích phân tích](#Mục-đích-phân-tích)
- [Thu thập dữ liệu](#Thu-thập-dữ-liệu)
- [Công nghệ sử dụng](#Công-nghệ-sử-dụng)
- [Giải thích cấu trúc](#Giải-thích-cấu-trúc)
- [Lời kết](#Lời-kết)

## Mục đích phân tích
Các ứng viên cho vị trí Business Analyst luôn dồi dào, và đều là những con người vô cùng tiềm năng. Họ dành những năm tháng đại học vô cùng nỗ lực để theo đuổi một nghề đòi hỏi 
sự tư duy cao, cũng như khả năng làm việc với khách hàng tốt. Công việc Business Analyst được coi là vô cùng quan trọng đối với doanh nghiệp, theo tác giả thấy, vì đây là công nghệ
mang tính chất cầu nối giữa con người với con người. Tôi có một cô bạn gái đang làm Business Analyst, và tôi cảm thấy cô ấy đang đóng góp vô cùng nhiều vào việc xây dựng hệ thống 
quản trị doanh nghiệp của công ty, cũng như làm cầu nối để công ty có thể hiểu được nghiệp vụ yêu cầu bởi các khách hàng.
<br>
<br>
Tuy vậy, một trong những cái đau đáu nhất của tác giả, kể cả trong những ngành nghề khác, đó là không biết bắt đầu từ đâu. Có lẽ các bạn sinh viên đang đeo đuổi một nghề nào đó, như DA, BA... đều đang vô cùng 
hoang mang. DA chỉ cần vẽ mấy cái chart, BA thì cần lắm mồm... và các bạn chẳng còn biết mình cần học gì để trở thành một người làm những công việc đó nữa. Không những vậy, lùa gà thì khắp mọi nơi, thi thoảng
lại một ẩn danh đăng tin tuyển dụng tiêu cực, thi thoảng lại có người nhận định thị trường xấu, lại người xuống bình luận gửi, spam một đống khóa học, trung tâm... Tôi căm ghét những con người đó vô cùng, chúng
lợi dụng tâm lý hoang mang của người mới bắt đầu, người không có thời gian tìm hiểu để quảng bá, tạo tiếng vang, tiếng lợi cho chúng.
<br>
<br>
Tôi cũng rất tự hào vì người yêu tôi rất giỏi, nhưng cô ấy muốn phát triển hơn nữa, dù gần như cô ấy biết mọi thứ về BA rồi, nhưng tham vọng phải luôn luôn là vô đáy. Vấn đề là công việc chiếm rất nhiều thời gian, lên mạng thì toàn mấy người đăng tin tiêu cực. Dĩ nhiên là người yêu tôi không tiêu cực, nhưng tôi ước mình có thể giúp cô ấy phần nào. Và thế là dự án này ra đời.
<br>
<br>
Tôi muốn các bạn sinh viên trẻ không còn hoang mang, hay những người bận rộn có thể biết tình hình thị trường mà không cần đọc từng tin tuyển dụng một. Tôi muốn họ tự tin, rằng nếu Intern không có job nào, thì bạn cần biết những kỹ năng đặc biệt này là lên thẳng Fresher làm luôn.

## Thu thập dữ liệu
Dữ liệu được cào về từ website TopCV sử dụng trình mở rộng 'Web Scraper' của Chrome. Xem thêm về trình mở rộng tại dưới này:
- [Trình mở rộng](https://chromewebstore.google.com/detail/web-scraper-free-web-scra/jnhgnonknehpejjnehehllkliplmbmhn)
- [Hướng dẫn sử dụng](https://www.youtube.com/@WebScraper)

Đây là dữ liệu về thị trường việc làm của <b> riêng nghề BA, tại thị trường Hà Nội, trong khoảng thời gian nhất định</b>. Làm ơn, lưu ý về đặc tả này.

## Công nghệ sử dụng
Các công nghệ được sử dụng trong bài bao gồm:
- Excel: chứa tệp dữ liệu gốc.
- Web Scraper: cào dữ liệu từ trang web.
- Python: công nghệ chính được sử dụng nhằm làm sạch, làm giàu dữ liệu lên rất nhiều.
- Mấy con AI: làm việc vặt như mapping, tạo dict...
- PowerBI: được sử dụng nhằm trực quan hóa dữ liệu và làm tinh gọn cơ sở dữ liệu, tối ưu năng suất hoạt động.
- Canva: công ty có tài khoản pro nên dùng ké, mục đích để tạo Infographics và kể chuyện qua dữ liệu hiệu quả hơn nữa.

## Giải thích cấu trúc
Các giải thích về cách đọc repo có thể được tìm thấy trong phần này.
1. File đầu tiên cần đọc là [origin-data](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/origin-data) để check dữ liệu gốc trông như thế nào, sạch sẽ ra sao. Điều khá bất ngờ là trên github dữ liệu gốc nhìn rất sạch, trong khi <b>tải về thì nhìn như gì</b>. Dữ liệu mà tác giả xử lý chính là dữ liệu nhìn như gì.
2. File thứ hai cần nhấp vào là [processing-with-python](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/processing-with-python) để xem quá trình làm sạch đã diễn ra như thế nào. Dự án này là dự án hoàn toàn có thể scale lên được, vì về sau tôi định quay lại và sử dụng .pipe() để tự động hóa code hơn nữa, nhìn ngắn cũn lại luôn, nhưng mà hiện tại thì nó là rất nhiều dòng code, đặc biệt là để nghĩ ra cách làm giàu dữ liệu hoặc biến cái dữ liệu trở nên ý nghĩa là phần cần nhiều suy nghĩ. Có vẻ cũng vì thiếu kinh nghiệm thôi.
3. File cuối cùng đó là [end-product](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product), file này chứa các sản phẩm thành quả và các folder con. Các folder như sau:
- [cleaned-data](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product/cleaned-data): chứa dữ liệu được làm sạch đã tách thành các bảng và cách các bảng này kết nối với nhau.
- [pbi-img](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product/pbi-img): lặt vặt thôi, chứa các ảnh sử dụng trong dự án.
- [infographics & power bi](https://github.com/hinmfm/Top-CV-BA-Job-Analysis/tree/main/end-product/infographics%20%26%20powerbi): chứa infographics và file Power BI để kể chuyện về dự án.
4. Mỗi file đều có kèm một <b>file README nên được đọc trước khi nghiên cứu các nội dung bên trong</b> file đó.

## Lời kết
Dự án được thực hiện trong vòng tổng cộng 3 ngày, nhưng vì bận công việc trên công ty nên phải 2 tuần sau dự án mới có đầy đủ mô tả =)))
<br>
<br>
Cảm ơn các độc giả đã đọc tới phần này của file. Cảm ơn hơn nữa nếu mọi người đã đọc hết.
<br>
<br>
<b>Liên hệ</b>: minhsatwork@gmail.com
