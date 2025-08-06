# Top-CV-BA-Job-Analysis
Dự án phân tích dữ liệu với dữ liệu được cào về từ Top CV nhằm phân tích tình hình thị trường công việc BA tại Hà Nội.
Dự án gồm các mục sau: 
1. [Mục đích phân tích](#Mục-đích-phân-tích) 
2. [Thu thập dữ liệu](#Thu-thập-dữ-liệu)
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
mang tính chất cầu nối giữa con người với con người. Bạn gái của tôi hiện đang làm Business Analyst, và tôi cảm thấy cô ấy đang đóng góp vô cùng nhiều không chỉ vào việc xây dựng hệ thống 
quản trị doanh nghiệp của công ty, mà còn là cầu nối để công ty có thể hiểu được nghiệp vụ yêu cầu bởi các khách hàng, và cả hiểu lẫn nhau.
<br>
<br>
Tuy vậy, một trong những chi tiết đau đáu nhất, kể cả trong những ngành nghề khác, đó là không biết bắt đầu từ đâu. Có lẽ các bạn sinh viên đang đeo đuổi một nghề nào đó, như DA, BA... đều vô cùng hoang mang. DA chỉ cần vẽ mấy cái chart, BA thì cần lắm mồm... và các bạn chẳng còn biết mình cần học gì để trở thành một người làm những công việc đó nữa. Không những vậy, lùa gà thì khắp mọi nơi, thi thoảng lại một ẩn danh đăng tin tuyển dụng tiêu cực, thi thoảng lại có người nhận định thị trường xấu, lại người xuống bình luận gửi, spam một đống khóa học, trung tâm... Tôi căm ghét những con người đó vô cùng, chúng lợi dụng tâm lý hoang mang của người mới bắt đầu, người không có thời gian tìm hiểu để quảng bá, tạo tiếng vang, tiếng lợi cho chúng.
<br>
<br>
Tôi cũng rất tự hào vì người yêu tôi rất giỏi, nhưng cô ấy muốn phát triển hơn nữa, dù gần như cô ấy biết mọi thứ về BA rồi, nhưng tham vọng phải luôn luôn là vô đáy. Vấn đề là công việc chiếm rất nhiều thời gian, lên mạng thì toàn mấy người đăng tin tiêu cực, nên làm sao biết được cần học cái gì nữa đây? Dĩ nhiên là người yêu tôi không tiêu cực, nhưng tôi ước mình có thể giúp cô ấy phần nào. Và thế là dự án này ra đời.
<br>
<br>
Tôi muốn các bạn sinh viên trẻ không hoang mang, hay những người bận rộn có thể biết tình hình thị trường mà không cần đọc từng tin tuyển dụng một. Tôi muốn họ tự tin, rằng nếu Intern không có job nào, thì bạn vẫn biết cần học cái gì để trở thành một Fresher.

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

## Bonus
Nếu đã đọc tới đây, các bạn sẽ phải nghe tôi tâm sự. Câu chuyện của tôi là một câu chuyện loằng ngoằng, dài thoòng. Tại sao á? Tôi đang là một DA, nhưng hành trình để tôi tới với nghề, được làm nghề nó rất khổ. Mặc dù ra trường thuộc hội sớm nhất từ tít tháng 2/2025, thành tích cũng ổn ổn (GPA: 3.54, song với trường kinh tế vậy là bình thường) nhưng tôi không thể kiếm nổi việc. Thực sự tôi đã nộp đơn từ năm ngoái tới năm hiện tại của dự án (2025), và tôi tính là đã có tới 64 lần hy vọng, 64 lần ứng tuyển.
<br>
<br>
62 lần tôi trượt. Tôi là một người mê mệt con số 8, và nếu đam mê thần số học qq gì đó, 6+2 lại là 8. Tôi tạch ở lần tôi tự coi là may mắn nhất. Thực sự thì khi tạch lần ứng tuyển thứ 62 tôi mông lung lắm rồi. Tôi vô vọng hoàn toàn, tôi lên mạng thì ai cũng nói DA thị trường nát rồi, rác rồi. Không có gì ngoài sự tiêu cực, ai cũng bảo chỉ tuyển Senior, rồi Intern trình Middle... đủ thứ trên đời. Và tôi lạc lõng. Tôi không quen ai làm DA hết, người quen cùng lớp thì từ chối giúp tôi, có lẽ cũng vì tính tôi tệ? Tất cả mọi thứ, đã đến từ chính tôi, chính sự nỗ lực của tôi. Tôi luôn phải tự nhủ bản thân rằng chính vì mình đang đi vào cái không ai làm được, nên làm được thì sẽ rất tuyệt vời. Nhưng mà sức ép xung quanh thì vẫn vậy, bạn bè thì thằng khoe nọ, thằng khoe kia, thằng đi làm được từng này rồi các thứ. Tôi nghĩ bụng biết thế hồi đó cũng xin người thân về quê cho làm logistics giống nó, chấp nhận mình ngu nhưng mà được cái có việc, oách, đăng lên mạng được.
<br>
<br>
62 lần đó là gần 1 năm của sự tự ti, tủi hổ. Tết cũng không thể vui vẻ nổi, gia đình du lịch tôi cũng ái ngại.
<br>
<br>
Nhưng đó cũng là 62 lần tự học. Đôi khi tôi nghĩ mình chưa thất bại bao giờ, vậy đây chính là cái cớ để thành công. Và lần 63 và 64 tôi đã pass, thậm chí tôi phỏng vấn 2 công ty cùng 1 ngày và pass cả 2 =))). Tôi cảm thấy mình vẫn rất may mắn, vì những lúc tôi chẳng còn điểm tựa chó nào, thì đã có tình yêu ở cạnh. Đó là tình yêu cuộc đời, yêu được làm DA và hơn cả, tình yêu từ gia đình và người yêu của mình. Trung tâm có tốt, có xấu. Nhưng tôi mong họ có trách nhiệm với hành động của mình, vì việc các bạn đăng tải tiêu cực lên, khiến mọi người lo sợ để bán mấy khóa học rẻ rách tiền triệu của mình cam kết 100% có việc làm, tôi nhổ vào bãi khóa học đó. Làm gì thì làm, đừng làm cho mọi thứ tiêu cực, đừng nói rằng nếu không làm A thì không thể làm B và đừng cam kết cái gì nếu không làm được. Tôi không bỏ tiền ra mua khóa nào của các bạn hết.
<br>
<br>
Cuộc đời tôi là chứng minh người khác sai. Nếu bạn là học sinh trường làng thì đừng mơ tiếng Anh giỏi, tôi đáp vào mồm trường chuyên 1 con 8.0 IELTS. Thực tập rất khó xin việc, đáp vào mồm họ job Fresher. DA khó xin việc, tôi đáp vào mồm họ 1 công việc. Mấy cái này nghe self-help thật, nhưng mà tôi chẳng bày cho các bạn làm cái này thì phải làm như này hay gì hết, tôi khuyến khích việc tự học, tự nghiên cứu trước khi làm bất cứ điều gì.
<br>
<br>
Nhưng thành thật mà nói, tôi từng súc vật hơn cả các bạn. Tôi chỉ không cần suy nghĩ mỗi cái không trả tiền thuê nhà hàng tháng thôi, cũng hơn khối người nhưng mà tôi cũng đã từng rất súc vật và khổ sở vì không xin được việc đấy. 
<br>
<br>
Vậy nên nỗ lực đi. Nỗ lực đi các bạn rồi sẽ thành công thôi.
