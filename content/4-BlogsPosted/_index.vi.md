---
title: "Các bài blog đã đăng"
date: 2026-07-29
weight: 4
chapter: false
pre: " <b> 4. </b> "
---

## Tổng quan

Trong quá trình thực hiện project, nhóm không chỉ xây dựng ứng dụng thực tế mà còn tổng hợp lại kiến thức thành các bài blog kỹ thuật. Các bài viết giúp hệ thống hóa quá trình phân tích bài toán, thiết kế giải pháp, triển khai backend/frontend và áp dụng tư duy bảo mật vào project **Cloud-based Student Internship Portal on AWS**.

Series blog tập trung vào cách **AWS Security Agent** có thể hỗ trợ nhóm phát triển trong nhiều giai đoạn khác nhau của vòng đời phần mềm: từ thiết kế kiến trúc, review mã nguồn cho đến kiểm thử khả năng chống chịu trước các tình huống tấn công thực tế.

## Danh sách bài blog

| Bài blog | Chủ đề | Nội dung chính | Giá trị học được | Liên kết |
| --- | --- | --- | --- | --- |
| Blog 1 | Xây dựng ứng dụng an toàn ngay từ bản thiết kế với AWS Security Agent | Trình bày lý do bảo mật cần được xem xét từ giai đoạn thiết kế, giới thiệu AWS Security Agent, Threat Modeling và cách áp dụng vào project Student Internship Portal. | Hiểu tư duy "Design for Security", cách phát hiện rủi ro kiến trúc sớm và cách cải thiện triển khai AWS an toàn hơn. | [Facebook post](https://www.facebook.com/groups/660548818043427?multi_permalinks=2227782947986665) |
| Blog 2 | AI Code Review với AWS Security Agent | Trình bày cách AWS Security Agent hỗ trợ phân tích mã nguồn, phát hiện rủi ro bảo mật trong API đăng nhập, upload CV và quản lý tin tuyển dụng trước khi triển khai. | Hiểu rằng ứng dụng chạy đúng chức năng chưa chắc đã an toàn, đồng thời nắm rõ hơn vai trò của secure coding và review code tự động. | [Facebook post](https://www.facebook.com/groups/660548818043427/?multi_permalinks=2228768907888069) |
| Blog 3 | Penetration Testing với AWS Security Agent | Trình bày cách sử dụng AI để hỗ trợ lập kế hoạch và đánh giá các kịch bản kiểm thử bảo mật trước khi ứng dụng được phát hành. | Hiểu vai trò của penetration testing trong quy trình DevSecOps và cách ưu tiên xử lý các rủi ro có khả năng bị khai thác trong thực tế. | [Facebook post](https://www.facebook.com/groups/awsstudygroupfcj/posts/2229167591181534/?notif_id=1785413805425251&notif_t=group_post_approved&ref=notif) |

## Blog 1 - Xây dựng ứng dụng an toàn ngay từ bản thiết kế với AWS Security Agent

Bài blog đầu tiên thuộc series **AWS Security Agent**, tập trung vào ý tưởng rằng bảo mật không nên chỉ bắt đầu sau khi ứng dụng đã hoàn thành. Một thiết kế tốt ngay từ đầu có thể giúp nhóm phát triển phát hiện và loại bỏ nhiều rủi ro trước khi chúng trở thành lỗi trong mã nguồn hoặc trong môi trường triển khai.

Nội dung bài viết nhấn mạnh rằng nhiều lỗ hổng bảo mật không xuất phát trực tiếp từ lỗi lập trình, mà đến từ các quyết định kiến trúc ban đầu. Ví dụ, database có thể bị đặt trong vùng mạng truy cập được từ Internet, API chưa có cơ chế xác thực phù hợp, hoặc các dịch vụ AWS được cấp quyền vượt quá nhu cầu thực tế. Nếu các vấn đề này chỉ được phát hiện sau khi hệ thống đã hoàn thiện, việc sửa đổi thường tốn nhiều thời gian và chi phí hơn.

### AWS Security Agent

Bài viết giới thiệu **AWS Security Agent** như một trợ lý AI hỗ trợ nhóm phát triển đánh giá mức độ an toàn của hệ thống ngay từ giai đoạn thiết kế. Thay vì chỉ quét lỗi trong mã nguồn, Security Agent có thể phân tích tài liệu thiết kế, sơ đồ kiến trúc, luồng dữ liệu, cấu hình triển khai AWS và mối quan hệ giữa các dịch vụ.

Từ đó, công cụ có thể giúp xác định những điểm có nguy cơ mất an toàn và đề xuất biện pháp cải thiện trước khi nhóm bắt đầu viết mã hoặc triển khai hệ thống. Điều này thể hiện sự chuyển đổi tư duy từ **Fix Security** sang **Design for Security**.

### Threat Modeling

Một phần quan trọng của bài viết là **Threat Modeling**, tức quá trình phân tích hệ thống để xác định các mối đe dọa tiềm ẩn. Quá trình này giúp trả lời các câu hỏi như hệ thống cần được bảo vệ khỏi những nguy cơ nào, thành phần nào dễ bị tấn công, kẻ tấn công có thể khai thác hệ thống theo hướng nào và thiết kế cần thay đổi ra sao để giảm thiểu rủi ro.

AWS Security Agent không thay thế chuyên gia bảo mật, nhưng có thể hỗ trợ nhóm phát triển phát hiện sớm các vấn đề về kiến trúc trước khi chúng trở thành lỗ hổng trong sản phẩm thực tế.

### Liên hệ với project Student Internship Portal

Bài viết áp dụng các ý tưởng trên vào dự án **Cloud-based Student Internship Portal on AWS**. Hệ thống sử dụng các dịch vụ như Amazon CloudFront, Amazon S3, Amazon EC2, Amazon RDS PostgreSQL, AWS IAM và Amazon CloudWatch. Khi nhìn dưới góc độ bảo mật, nhóm cần xem xét các câu hỏi như RDS có nằm trong private subnet hay không, EC2 có mở SSH cho toàn bộ Internet không, IAM Role có bị cấp quá nhiều quyền không và dữ liệu trao đổi giữa các thành phần đã được mã hóa hay chưa.

Một ví dụ cụ thể là việc triển khai Amazon RDS với cấu hình public access để thuận tiện trong giai đoạn phát triển. Về chức năng, hệ thống vẫn có thể hoạt động bình thường, nhưng dưới góc nhìn bảo mật, đây là một rủi ro lớn. AWS Security Agent có thể khuyến nghị đưa RDS vào private subnet, chỉ cho phép EC2 truy cập thông qua Security Group và loại bỏ truy cập trực tiếp từ Internet.

### Bài học chính

Thông qua bài blog này, em rút ra rằng một kiến trúc tốt không chỉ là kiến trúc hoạt động đúng chức năng, mà còn phải an toàn, dễ kiểm soát và có khả năng giảm thiểu rủi ro từ sớm. Việc đánh giá bảo mật ngay từ giai đoạn thiết kế giúp giảm chi phí sửa lỗi, hỗ trợ nhóm phát triển hiểu rõ hơn tác động của từng quyết định kiến trúc và đặt nền tảng cho tư duy DevSecOps trong các giai đoạn tiếp theo.

Link bài đăng: [Facebook post](https://www.facebook.com/groups/660548818043427?multi_permalinks=2227782947986665)

## Blog 2 - AI Code Review với AWS Security Agent

Bài blog thứ hai trong series **AWS Security Agent** tập trung vào giai đoạn sau khi hệ thống đã có thiết kế ban đầu: kiểm tra mã nguồn trước khi ứng dụng được triển khai. Nội dung chính của bài viết là việc một ứng dụng hoạt động đúng chức năng chưa có nghĩa là ứng dụng đó đã đủ an toàn trước các rủi ro thực tế.

Bài viết nhấn mạnh rằng nhiều lỗ hổng bảo mật thường xuất hiện trong quá trình lập trình. Một API có thể chạy đúng theo yêu cầu nghiệp vụ nhưng vẫn tồn tại lỗi xác thực, xử lý dữ liệu đầu vào chưa đầy đủ, phân quyền chưa chặt chẽ hoặc ghi log chứa thông tin nhạy cảm. Những vấn đề này thường khó phát hiện nếu chỉ kiểm thử chức năng thông thường.

### AI Code Review

AI Code Review là quá trình sử dụng trí tuệ nhân tạo để phân tích mã nguồn, xác định rủi ro bảo mật và đề xuất cách cải thiện. Khác với công cụ kiểm tra cú pháp hoặc định dạng code, AI Code Review cố gắng hiểu ngữ cảnh của ứng dụng, bao gồm luồng xử lý, dữ liệu truyền qua API, quy trình xác thực, cơ chế phân quyền và cách ứng dụng tương tác với database hoặc dịch vụ bên ngoài.

Với AWS Security Agent, quá trình review có thể được áp dụng trên Pull Request hoặc trên toàn bộ project. Agent có thể đọc phần mã mới, xác định điểm có nguy cơ mất an toàn, giải thích nguyên nhân, đánh giá mức độ ảnh hưởng và đề xuất hướng khắc phục phù hợp.

### Liên hệ với project Student Internship Portal

Bài viết sử dụng dự án **Cloud-based Student Internship Portal on AWS** để minh họa các tình huống bảo mật thường gặp trong code.

Với **API đăng nhập**, AWS Security Agent có thể kiểm tra các rủi ro như JWT có thời gian sống quá dài, thiếu cơ chế giới hạn số lần đăng nhập thất bại, mật khẩu chưa được xử lý đúng cách hoặc thông báo lỗi tiết lộ quá nhiều thông tin. Ví dụ, nếu hệ thống trả về riêng biệt hai lỗi "Email không tồn tại" và "Sai mật khẩu", kẻ tấn công có thể lợi dụng để xác định tài khoản hợp lệ. Cách xử lý an toàn hơn là dùng thông báo chung như "Email hoặc mật khẩu không chính xác".

Với **API upload CV**, việc upload file thành công chưa đủ để kết luận chức năng an toàn. Hệ thống cần kiểm tra loại file, kích thước file, tên file, nội dung thực tế của file và cách lưu trữ trên S3. AWS Security Agent có thể gợi ý bổ sung các bước kiểm tra để giảm nguy cơ người dùng tải lên file độc hại hoặc file không đúng định dạng.

Với **API quản lý tin tuyển dụng**, một lỗi phổ biến là chỉ kiểm tra người dùng đã đăng nhập mà chưa kiểm tra quyền sở hữu dữ liệu. Điều này có thể dẫn đến tình huống một doanh nghiệp chỉnh sửa hoặc xóa bài đăng của doanh nghiệp khác. Agent có thể phát hiện các đoạn code thiếu kiểm tra quyền và đề xuất bổ sung bước xác minh owner trước khi thực hiện thao tác.

### Giá trị của AWS Security Agent

Điểm quan trọng của AWS Security Agent không chỉ là phát hiện đoạn code có vấn đề, mà còn giải thích vì sao đó là rủi ro, mức độ ảnh hưởng nếu bị khai thác, cách kẻ tấn công có thể lợi dụng và hướng khắc phục phù hợp. Điều này giúp quá trình review code trở thành một hoạt động học tập về secure coding, đặc biệt hữu ích với nhóm phát triển chưa có nhiều kinh nghiệm bảo mật.

### Bài học chính

Thông qua bài blog này, em rút ra rằng kiểm thử chức năng và kiểm tra bảo mật là hai góc nhìn khác nhau. Một chức năng đăng nhập, upload CV hoặc quản lý bài tuyển dụng có thể chạy đúng nhưng vẫn cần được review kỹ về xác thực, phân quyền, validation, logging và kiểm soát dữ liệu. Việc tích hợp AI Code Review vào quy trình phát triển giúp phát hiện rủi ro sớm hơn, giảm chi phí sửa lỗi và nâng cao chất lượng mã nguồn trước khi triển khai.

Link bài đăng: [Facebook post](https://www.facebook.com/groups/660548818043427/?multi_permalinks=2228768907888069)

## Blog 3 - Penetration Testing với AWS Security Agent

Bài blog thứ ba trong series **AWS Security Agent** tập trung vào giai đoạn kiểm tra cuối cùng trước khi hệ thống được đưa vào vận hành: **Penetration Testing**. Nếu hai bài trước giúp nhóm phát triển xây dựng ứng dụng an toàn từ thiết kế và mã nguồn, thì bài thứ ba đặt ra câu hỏi thực tế hơn: nếu một hacker thật sự cố gắng tấn công ứng dụng, điều gì sẽ xảy ra?

Penetration Testing là quá trình mô phỏng các cuộc tấn công có chủ đích nhằm đánh giá khả năng bảo vệ của một hệ thống. Khác với việc quét lỗ hổng tự động, Pentest không chỉ hỏi hệ thống có rủi ro nào hay không, mà còn đánh giá liệu rủi ro đó có thể bị khai thác thành công và gây ảnh hưởng thực tế đến ứng dụng hay không.

### AWS Security Agent hỗ trợ Penetration Testing

AWS Security Agent có thể hỗ trợ nhóm phát triển lập kế hoạch và đánh giá các kịch bản kiểm thử bảo mật dựa trên bối cảnh của toàn bộ ứng dụng. Agent xem xét nhiều thành phần như kiến trúc hệ thống, API, luồng xác thực, cơ chế phân quyền, thành phần lưu trữ dữ liệu và cấu hình triển khai trên AWS.

Từ những thông tin này, Agent có thể đề xuất các tình huống kiểm thử phù hợp, xác định những điểm cần ưu tiên đánh giá và giúp nhóm phát triển tập trung vào các rủi ro có khả năng gây ảnh hưởng lớn nhất. Mục tiêu của AWS Security Agent không phải thay thế chuyên gia Pentest, mà là giúp quá trình kiểm thử có trọng tâm và hiệu quả hơn.

### Các kịch bản áp dụng cho Student Internship Portal

Với dự án **Cloud-based Student Internship Portal**, bài viết đưa ra nhiều kịch bản kiểm thử thực tế trước khi phát hành phiên bản đầu tiên.

Kịch bản đầu tiên là **truy cập trái phép hồ sơ ứng tuyển**. Mỗi sinh viên chỉ nên xem thông tin và hồ sơ của chính mình. Nếu người dùng thay đổi tham số trong URL hoặc API để xem dữ liệu của người khác, hệ thống có thể gặp lỗi kiểm soát truy cập kiểu **Insecure Direct Object Reference (IDOR)**. AWS Security Agent có thể nhắc nhóm kiểm tra việc xác minh quyền sở hữu dữ liệu trước khi trả về kết quả.

Kịch bản thứ hai là **tải lên tệp độc hại**. Vì hệ thống cho phép sinh viên upload CV dưới dạng PDF, ứng dụng không nên chỉ kiểm tra phần mở rộng của file. Hệ thống cần kiểm tra loại file thực tế, giới hạn kích thước, đổi tên file khi lưu trữ và quét nội dung trước khi cho phép truy cập.

Kịch bản thứ ba là **tấn công đăng nhập tự động**. Nếu API đăng nhập không giới hạn số lần thử hoặc không có cơ chế làm chậm yêu cầu, kẻ tấn công có thể dùng công cụ tự động để thử nhiều mật khẩu trên cùng một tài khoản. AWS Security Agent có thể gợi ý bổ sung rate limiting, khóa tạm thời tài khoản sau nhiều lần đăng nhập thất bại, theo dõi mẫu truy cập bất thường và gửi cảnh báo khi phát hiện dấu hiệu tấn công.

Kịch bản thứ tư là **cấu hình AWS chưa phù hợp**. Không phải mọi rủi ro đều đến từ mã nguồn. Amazon RDS có thể bị cấu hình public access, Security Group có thể mở nhiều cổng không cần thiết, IAM Role có thể được cấp quyền vượt quá nhu cầu hoặc CloudWatch Logs chưa được bật đầy đủ. Những cấu hình này cần được rà soát trước khi triển khai chính thức.

### Penetration Testing không chỉ là tìm lỗi

Bài viết nhấn mạnh rằng Pentest không chỉ nhằm phát hiện càng nhiều lỗi càng tốt. Giá trị quan trọng hơn là hiểu lỗ hổng nào thật sự có thể bị khai thác, mức độ ảnh hưởng đến hệ thống, thành phần nào cần ưu tiên khắc phục và giải pháp nào mang lại hiệu quả cao nhất.

Khi nhìn lại toàn bộ series, AWS Security Agent đã đồng hành với project ở ba giai đoạn: **Security by Design**, **Secure Coding** và **Penetration Testing**. Ba giai đoạn này tạo thành một quy trình bảo mật xuyên suốt, thay vì xem bảo mật là một bước kiểm tra riêng lẻ ở cuối dự án.

### Bài học chính

Thông qua bài blog này, em rút ra rằng bảo mật không phải là một tính năng có thể bổ sung sau khi ứng dụng hoàn thành. Một hệ thống an toàn cần được hình thành từ nhiều quyết định đúng đắn trong suốt vòng đời phát triển: thiết kế kiến trúc hợp lý, viết mã theo nguyên tắc secure coding và chủ động kiểm thử bằng các tình huống tấn công trước khi triển khai.

Đối với dự án **Cloud-based Student Internship Portal**, việc áp dụng tư duy này không chỉ giúp bảo vệ dữ liệu của sinh viên và doanh nghiệp, mà còn xây dựng nền tảng cho một quy trình DevSecOps hiện đại, nơi bảo mật trở thành trách nhiệm chung trong toàn bộ quá trình phát triển phần mềm.

Link bài đăng: [Facebook post](https://www.facebook.com/groups/awsstudygroupfcj/posts/2229167591181534/?notif_id=1785413805425251&notif_t=group_post_approved&ref=notif)

## Nội dung rút ra

Thông qua việc viết blog, em có cơ hội nhìn lại toàn bộ quá trình làm project một cách có hệ thống hơn. Thay vì chỉ tập trung vào code, em phải diễn giải rõ vấn đề, lý do chọn công nghệ, cách các thành phần kết nối với nhau và kết quả đạt được sau khi triển khai.

Series **AWS Security Agent** cũng giúp em hiểu rõ hơn rằng bảo mật cần được tích hợp xuyên suốt vòng đời phát triển phần mềm. Từ thiết kế kiến trúc, review mã nguồn đến penetration testing, mỗi giai đoạn đều góp phần giảm thiểu rủi ro và giúp ứng dụng sẵn sàng hơn khi vận hành trong môi trường thực tế.

Hoạt động này giúp em cải thiện khả năng trình bày kỹ thuật, viết tài liệu, chọn lọc thông tin quan trọng và giải thích một giải pháp công nghệ theo cách dễ hiểu hơn cho người đọc.
