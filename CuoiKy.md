# A wilderness weather station
## I.Mô tả tóm tắt bài toán:
### 1.Mục tiêu của bài toán:
Xây dựng hệ thống trạm thời tiết tự động hoạt động trong các khu vực vùng sâu, vùng xa, không có cơ sở hạ tầng hỗ trợ (điện, đường giao thông, mạng viễn thông). Hệ thống này có nhiệm vụ thu thập, xử lý và truyền dữ liệu thời tiết về trung tâm để phục vụ:
- Nghiên cứu và phân tích biến đổi khí hậu ở cả cấp địa phương và quốc gia.
- Nâng cao độ chính xác của dự báo thời tiết quốc gia.
- Hỗ trợ quản lý tài nguyên thiên nhiên và phòng chống thiên tai.
### 2.Các đặc điểm chính của hệ thống:
#### 2.1.Tự cấp nguồn năng lượng:
- Sử dụng năng lượng tái tạo (năng lượng mặt trời hoặc gió) để vận hành toàn bộ hệ thống, không phụ thuộc vào nguồn điện bên ngoài.
#### 2.2.Giao tiếp từ xa qua vệ tinh:
- Truyền dữ liệu thời tiết về hệ thống trung tâm và nhận cập nhật phần mềm hoặc cấu hình từ xa.
#### 2.3.Hoạt động tự động và đáng tin cậy:
- Hệ thống phải hoạt động độc lập trong thời gian dài, có khả năng tự xử lý lỗi cơ bản và tự khởi động lại khi cần.
#### 2.4.Tự cấu hình và nâng cấp từ xa:
- Cho phép thay đổi cấu hình hoặc cập nhật phần mềm từ xa mà không cần truy cập trực tiếp.
### 3.Sự cần thiết và lợi ích khi giải quyết bài toán:
Trạm thời tiết vùng hoang dã là một thành phần quan trọng trong hệ thống thu thập thông tin thời tiết quốc gia. Việc xây dựng và triển khai trạm thời tiết tự động ở những khu vực không có cơ sở hạ tầng (điện, mạng, đường xá, v.v.) mang lại những lợi ích sau:
- Hỗ trợ nghiên cứu biến đổi khí hậu: Dữ liệu từ các trạm thời tiết giúp phân tích biến đổi khí hậu cục bộ và quốc gia, hỗ trợ các nhà khoa học đưa ra các dự báo chính xác hơn về xu hướng thời tiết trong tương lai.
- Cung cấp thông tin dự báo thời tiết: Các trạm này đóng góp vào hệ thống dự báo thời tiết quốc gia, phục vụ cho các hoạt động dự báo và cảnh báo sớm, đặc biệt là trong những tình huống thiên tai như bão, lũ lụt, hay hạn hán.
- Quản lý tài nguyên tự nhiên và giảm thiểu rủi ro thiên tai: Dữ liệu thời tiết có thể giúp các nhà khoa học và cơ quan chính phủ quản lý nguồn tài nguyên hiệu quả và phản ứng nhanh với các sự kiện thời tiết cực đoan.
### 4.Các yêu cầu chức năng:
#### 4.1.Thu thập và xử lý dữ liệu thời tiết:
- Trạm cần có khả năng đo và lưu trữ các thông số thời tiết như nhiệt độ, độ ẩm, áp suất không khí, tốc độ và hướng gió, lượng mưa.
- Dữ liệu phải được xử lý sơ bộ trước khi gửi về hệ thống trung tâm qua vệ tinh.
#### 4.2.Lưu trữ và xử lý dữ liệu:
- Hệ thống cần khả năng lưu trữ dữ liệu thu thập được trong bộ nhớ tạm thời, và sau đó gửi dữ liệu này lên hệ thống trung tâm khi có kết nối.
#### 4.3.Kết nối và truyền tải dữ liệu:
- Khi có tín hiệu vệ tinh hoặc mạng không dây, trạm cần có khả năng truyền tải dữ liệu về trung tâm để phân tích và sử dụng cho các mục đích dự báo.
#### 4.4.Quản lý năng lượng:
- Trạm cần có khả năng tự tạo điện năng từ nguồn năng lượng tái tạo như tấm pin mặt trời hoặc năng lượng gió và có hệ thống quản lý năng lượng hiệu quả để đảm bảo hoạt động liên tục.
#### 4.5.Khả năng tự động điều chỉnh và cấu hình lại:
- Hệ thống phần mềm cần có khả năng tự cấu hình lại để đối phó với các lỗi thiết bị, thay đổi trong môi trường, hoặc nâng cấp phần mềm từ xa.
#### 4.6.Bảo mật và độ tin cậy:
- Đảm bảo rằng dữ liệu được thu thập và truyền tải một cách an toàn, không bị tấn công hoặc giả mạo.
### 5.Các Yêu Cầu Phi Chức Năng:
Các yêu cầu phi chức năng cho hệ thống trạm thời tiết hoang dã chủ yếu tập trung vào khả năng hoạt động độc lập và tính bền vững của hệ thống:
#### 5.1.Tính độc lập và tự chủ:
- Vì các trạm thời tiết được triển khai ở những khu vực xa xôi, không có cơ sở hạ tầng, hệ thống phải hoạt động hoàn toàn độc lập. Điều này bao gồm tự cung cấp năng lượng, tự duy trì và tự khởi động lại sau sự cố.
#### 5.2.Khả năng chống chịu môi trường khắc nghiệt:
- Trạm cần phải có thiết kế bền vững để chịu được các điều kiện môi trường khắc nghiệt như gió mạnh, mưa lớn, nhiệt độ cực đoan, và các yếu tố tự nhiên khác.
#### 5.3.Tiết kiệm năng lượng:
- Với nguồn năng lượng hạn chế từ năng lượng tái tạo, trạm phải có khả năng tối ưu hóa việc sử dụng năng lượng để duy trì hoạt động liên tục trong điều kiện ít ánh sáng mặt trời hoặc gió
#### 5.4.Khả năng mở rộng:
- Hệ thống cần có khả năng dễ dàng mở rộng và thêm mới các trạm thời tiết mà không cần thay đổi cấu trúc hoặc phần mềm hệ thống hiện tại.
#### 5.5.Bảo trì và sửa chữa dễ dàng:
- Dù khó tiếp cận, nhưng hệ thống phần cứng và phần mềm của trạm cần phải thiết kế sao cho dễ bảo trì và sửa chữa từ xa, chẳng hạn như khả năng tự chẩn đoán sự cố và cập nhật phần mềm từ xa.

## II.Phân tích các ca sử dụng:
### 1. Kiến trúc đề xuất:
Hệ thống được thiết kế theo kiến trúc hướng đối tượng (object-oriented architecture) với các thành phần chính sau:
- Lớp cảm biến (Sensors):
  - Thu thập dữ liệu thời tiết từ các cảm biến như nhiệt độ, độ ẩm, tốc độ gió, áp suất không khí, lượng mưa.
  - Gửi dữ liệu thô đến lớp xử lý.

- Lớp xử lý dữ liệu (Data Processor):
  - Xử lý dữ liệu thô từ cảm biến, bao gồm làm sạch dữ liệu, phát hiện lỗi, và chuẩn bị dữ liệu để gửi đi.
  - Phân loại và lưu trữ dữ liệu tạm thời trong bộ nhớ.

- Lớp quản lý năng lượng (Power Management):
  - Theo dõi và quản lý việc tiêu thụ năng lượng của hệ thống.
  - Điều phối hoạt động của các thành phần dựa trên mức năng lượng hiện có từ nguồn tái tạo.

- Lớp truyền thông (Communication):
  - Kết nối với hệ thống vệ tinh để truyền dữ liệu về trung tâm.
  - Nhận lệnh hoặc bản cập nhật phần mềm từ trung tâm.

- Lớp quản lý lỗi (Fault Management):
  - Phát hiện lỗi phần cứng hoặc phần mềm và kích hoạt cơ chế khắc phục (tự cấu hình lại hoặc thông báo lỗi).

- Lớp điều khiển chính (Main Controller):
  - Điều phối hoạt động của các lớp trên, đảm bảo hệ thống hoạt động liên tục và chính xác.

### Biểu đồ kiến trúc đơn giản:
![Login](https://www.planttext.com/plantuml/png/ZLGzRnD14ErFklymFR54xG854X4X9SWeAMZNvvDlbTjPixSB14GHKQIWmK88KL0aLgeeIb12SokKugpyZ_qdxAxlOj-79LoSvDityzxCUtkRcIH2AfQ6GNP8SK84OH2b9CkUIYdeKCduHSHndtw8uN4OX84_Wpr2SOkZ53nDOm4Vmm3ixn7ClrAZZnLC4gEd519kybC9ywdHFt6y19bync1ednoC_euUy0KJi5Kd85sjGtzQykt7c76HxPAZLRQ3H3bqVZc1aT5Na5ho4_zA_w8WgSdlP8NTCVgIDc35hMFExn2sYIG3mQCuipIUfKRVFbwAU6qRGrhyRVMk08Eai3j8t052QlGFMftitbzRg71rqYwAbShNItvVSPMojpXZ2cb49ENObZtWxsAnHv2COnQZR6qlvZ0g_b30-MSSGtf_RVHiQPFLVOQLazqGg_0RwyE1oSyPJ2XkW5IaDwG8OrhSRBXNhgOSigQjBNr5cL17DaPOc_sD8l3MvuDYKY5VElSH8fy1T7-aNQM-i8JAwfN56QknFYSgbMitiaCBQqBcxF8-DV9OYZFwDnnQggl8B-SygfkwS6rOd7A8t6FHoIe_RejgNADUxqazwVt6XUgiw0ZdVzLrfgCFhvIzb-XJrZIzeqc7ZKroD_R2JdShrlJfDARLwI7_vSR3eBQkjTlORbtD3jZQSLQhvzDYzY0Z33fbkqQD4Vlmh1u8ftqpnf7_ylu3)


### 2.Các cơ chế phân tích:
#### 2.1.Cơ chế làm sạch dữ liệu (Data Cleaning): Làm sạch dữ liệu thu thập từ các cảm biến, loại bỏ các giá trị nhiễu hoặc không hợp lệ.
##### Phân tích cơ chế:
- Các cảm biến thu thập dữ liệu có thể gặp sự cố hoặc bị nhiễu do môi trường (ví dụ: cảm biến nhiệt độ bị ảnh hưởng bởi ánh sáng mặt trời trực tiếp hoặc cảm biến gió bị ảnh hưởng bởi các vật cản).
- Data Cleaning đảm bảo rằng dữ liệu đầu vào là chính xác và có thể sử dụng cho các phân tích sau này.
- Lợi ích: Giúp đảm bảo chất lượng dữ liệu đầu vào, từ đó cải thiện độ chính xác của dự báo thời tiết và các nghiên cứu về biến đổi khí hậu.
##### Các hoạt động chính:
- Loại bỏ các giá trị cực trị hoặc không hợp lý (ví dụ: nhiệt độ cực cao hoặc thấp).
- Chuẩn hóa dữ liệu từ các cảm biến khác nhau (ví dụ: chuyển đổi đơn vị đo lường nếu cần).

#### 2.2.Cơ chế phát hiện lỗi (Error Detection): Phát hiện các lỗi phần cứng hoặc lỗi dữ liệu bất thường trong hệ thống.
##### Phân tích cơ chế:
-Trạm thời tiết làm việc trong môi trường khắc nghiệt và xa xôi, vì vậy việc phát hiện lỗi kịp thời là rất quan trọng.
- Error Detection đảm bảo hệ thống có thể xác định các vấn đề như:
    - Lỗi phần cứng (ví dụ: cảm biến không hoạt động).
    - Dữ liệu bất thường hoặc bị lỗi (ví dụ: cảm biến bị hỏng hoặc gặp sự cố truyền thông).
- Lợi ích: Phát hiện lỗi sớm sẽ giúp tiết kiệm thời gian và chi phí sửa chữa, đồng thời duy trì tính ổn định của hệ thống.
##### Các hoạt động chính:
- Giám sát trạng thái các cảm biến và các thành phần hệ thống.
- So sánh dữ liệu thu thập được với các mô hình dự đoán (như mô hình khí hậu cơ bản) để phát hiện sự bất thường.

#### 2.3.Cơ chế giám sát năng lượng (Energy Monitoring): Theo dõi và quản lý mức năng lượng sử dụng của hệ thống.
##### Phân tích cơ chế:
- Trạm thời tiết cần hoạt động hoàn toàn tự động và không phụ thuộc vào nguồn năng lượng từ bên ngoài. Do đó, Energy Monitoring đóng vai trò quan trọng trong việc đảm bảo nguồn năng lượng luôn đủ để duy trì hoạt động của các cảm biến, bộ xử lý và hệ thống truyền thông.
- Lợi ích: Đảm bảo rằng hệ thống có đủ năng lượng để hoạt động liên tục, đặc biệt trong các điều kiện khắc nghiệt (ví dụ: thời tiết xấu, không có ánh sáng mặt trời).
- Các yếu tố năng lượng như tấm pin mặt trời, tua-bin gió và pin lưu trữ phải được theo dõi và điều phối để tối ưu hóa hiệu suất.
##### Các hoạt động chính:
- Theo dõi mức năng lượng từ các nguồn cung cấp (năng lượng mặt trời, gió, pin).
- Ước tính mức tiêu thụ năng lượng và cảnh báo khi mức năng lượng giảm xuống dưới ngưỡng tối thiểu.

#### 2.4.Cơ chế tự động cấu hình lại (Auto Reconfiguration): Khôi phục hoạt động của hệ thống khi phát hiện lỗi nhỏ hoặc sự cố.
##### Phân tích cơ chế:
- Hệ thống trạm thời tiết hoạt động ở những khu vực xa xôi, khó tiếp cận, do đó, việc sửa chữa hoặc can thiệp trực tiếp sẽ rất khó khăn.
- Auto Reconfiguration giúp hệ thống tự động khôi phục hoặc tái cấu hình khi gặp sự cố nhỏ (ví dụ: cảm biến bị hỏng, hoặc phần mềm gặp lỗi).
- Lợi ích: Tiết kiệm chi phí và thời gian, duy trì hoạt động của hệ thống mà không cần phải sửa chữa trực tiếp.
##### Các hoạt động chính:
- Cấu hình lại các thành phần hệ thống khi phát hiện lỗi nhỏ.
- Khởi động lại các cảm biến hoặc bộ phận bị lỗi mà không cần can thiệp từ xa.

#### 2.5.Cơ chế truyền thông qua vệ tinh (Satellite Communication): Đảm bảo việc truyền tải dữ liệu từ hệ thống trạm thời tiết đến trung tâm điều hành và nhận cập nhật từ trung tâm.
##### Phân tích cơ chế:
- Hệ thống cần truyền tải dữ liệu thời tiết thu thập được đến các trung tâm điều hành qua vệ tinh, vì khu vực lắp đặt không có cơ sở hạ tầng truyền thông.
- Satellite Communication cung cấp kênh truyền thông cần thiết cho hệ thống, giúp dữ liệu được truyền tải an toàn và hiệu quả.
- Lợi ích: Giúp hệ thống duy trì kết nối liên tục dù ở khu vực xa xôi, giúp cập nhật thông tin kịp thời và nhận các bản cập nhật hoặc lệnh từ trung tâm.
##### Các hoạt động chính:
- Truyền dữ liệu thu thập về trung tâm.
- Nhận các lệnh hoặc bản cập nhật phần mềm từ trung tâm.

#### 2.6.Cơ chế lưu trữ tạm thời (Temporary Storage): Lưu trữ tạm thời dữ liệu trước khi xử lý hoặc gửi đi.
##### Phân tích cơ chế:
- Dữ liệu từ các cảm biến cần được lưu trữ tạm thời để xử lý trước khi gửi đi hoặc khi cần thực hiện các phép tính phân tích.
- Temporary Storage giúp lưu trữ và giữ dữ liệu an toàn cho đến khi được xử lý hoặc truyền đi.
- Lợi ích: Đảm bảo rằng dữ liệu không bị mất trong trường hợp có sự cố và có thể được truy xuất lại khi cần thiết.
##### Các hoạt động chính:
- Lưu trữ dữ liệu trong bộ nhớ tạm thời trước khi gửi đi.
- Quản lý dung lượng bộ nhớ để tối ưu hóa việc lưu trữ.

### Biểu đồ quan hệ của các cơ chế:
![Login](https://www.planttext.com/plantuml/png/VLJBRjD05DrRyZ_SFQh4EWlKaY90F8H85smdpk0PrPunanc9WbXLA0iM9Ik4K0MXYX2Fg4M8ZKU8XQFyn_m9Tvn7FKbA5exjkVUSUyyvoMvV4wLDdiLH_v2BWYYIGvAHVdzFQyMxHjExYHGT_eB2zJYAe_eCzeacxOmImKKAB-C8y7CDxajNZZXqdJs1dhFda75d1mO4m-_NPbdMPiQLNmMmwXTfriNHgqk6Mqf9jKyrJJINufBZ4Qj66ZpWG43cx3iEYIlFSkXoL_uL_obhJjHrvLY3PhCBPqz56Z8BgjAZ1r9mBLMmtm6Z4dhLRmvYUem7cMy_mvi5Z_RhBujdvyv-I41N4y7MwpMllXcaTtOSKEyPBHzJrFifJuqYuUO7plw4wT3PzuY0EuyDAlW3mRDQTGGRr913F3vaVB6rm3SdIuXx-F2Hhq3cZPfLdn2bOAxy8hnvR-QjmMGTeccMSKtRCi-DuCdQSBUTdOGI8mdw0LePlt3rEL-MFaIYYV0RJ0e_NZb19vpz7fGsg0zeNaX5r547_I0fRUHjTc42Jcz0NejmklBX3kw2q2WyF3FL26zhqPxZm91LVxO4C0ZtpiwDzIosuCcoMIjlAThi1IysCXT7QwqURPl9BRXPZUJ2Cc_FyQR32BQUpAlXfc_dFmgyoetqAOdNfXXRkAumt3Dk6DBQuaHJcBGEntI8i1kz7Z0Gl0LjimXu4K0cJAvSypRjKj6h_xZ-0G00)

### 3.Kết quả các ca phân tích:
#### Ca sử dụng 1: Thu thập dữ liệu thời tiết
##### Mục tiêu: Thu thập dữ liệu về các yếu tố khí hậu (nhiệt độ, độ ẩm, áp suất không khí, tốc độ gió) từ các cảm biến trong khu vực.
- Mô tả:
  - Người tham gia: Cảm biến (sensors), hệ thống giám sát.
- Tiến trình:
  - Cảm biến đo lường các yếu tố khí hậu.
  - Dữ liệu thu thập được sẽ được chuyển tiếp đến DataProcessorLayer để làm sạch và xử lý.
- Kết quả: Dữ liệu thời tiết chính xác được thu thập và chuyển đến lớp xử lý.

#### Ca sử dụng 2: Xử lý dữ liệu và phát hiện lỗi
##### Mục tiêu: Xử lý dữ liệu thu thập được từ các cảm biến, đồng thời phát hiện lỗi trong quá trình thu thập.
- Mô tả:
  - Người tham gia: DataProcessorLayer, ErrorDetection.
- Tiến trình:
  - Dữ liệu thô được gửi đến DataProcessorLayer để làm sạch và xử lý.
  - ErrorDetection phát hiện lỗi dữ liệu hoặc phần cứng.
  - Nếu phát hiện lỗi, hệ thống sẽ gửi cảnh báo về FaultManagementLayer.
- Kết quả: Dữ liệu được xử lý và lỗi (nếu có) sẽ được phát hiện và báo cáo.
  
#### Ca sử dụng 3: Quản lý năng lượng
##### Mục tiêu: Quản lý nguồn năng lượng của hệ thống để đảm bảo hoạt động liên tục.
- Mô tả:
  - Người tham gia: PowerManagementLayer.
- Tiến trình:
  - EnergyMonitoring theo dõi tình trạng năng lượng của hệ thống.
  - Kiểm tra mức năng lượng từ các nguồn (pin mặt trời, tua-bin gió, pin lưu trữ).
  - Nếu mức năng lượng quá thấp, hệ thống sẽ kích hoạt chế độ tiết kiệm năng lượng hoặc gửi cảnh báo về trung tâm.
-Kết quả: Đảm bảo hệ thống luôn có đủ năng lượng hoạt động và không bị gián đoạn.

#### Ca sử dụng 4: Truyền tải dữ liệu qua vệ tinh
##### Mục tiêu: Truyền tải dữ liệu về trung tâm điều khiển để phân tích và lưu trữ.
- Mô tả:
  - Người tham gia: CommunicationLayer, SatelliteCommunication.
- Tiến trình:
  - Dữ liệu đã được xử lý sẽ được gửi qua vệ tinh đến trung tâm điều khiển.
  - Dữ liệu có thể là các thông tin thời tiết, báo cáo sự cố hoặc cập nhật từ hệ thống.
  - Trung tâm điều khiển sẽ nhận dữ liệu và đưa ra quyết định dựa trên thông tin nhận được.
- Kết quả: Dữ liệu được truyền đi thành công, đảm bảo việc theo dõi và phân tích từ xa.

#### Ca sử dụng 5: Phát hiện và xử lý lỗi tự động
##### Mục tiêu: Phát hiện lỗi trong hệ thống và tự động tái cấu hình để tiếp tục hoạt động.
- Mô tả:
  - Người tham gia: FaultManagementLayer, AutoReconfiguration.
- Tiến trình:
  - FaultManagementLayer giám sát và phát hiện các lỗi hệ thống (cảm biến không hoạt động, mất kết nối, lỗi dữ liệu).
  - AutoReconfiguration tự động khôi phục hệ thống khi có lỗi nhỏ, chẳng hạn như tái khởi động lại cảm biến hoặc hệ thống.
  - Nếu lỗi không thể tự động xử lý, hệ thống sẽ gửi cảnh báo về trung tâm điều khiển.
- Kết quả: Hệ thống khôi phục hoạt động hoặc cảnh báo về lỗi nghiêm trọng.

#### Ca sử dụng 6: Lưu trữ tạm thời dữ liệu
##### Mục tiêu: Lưu trữ dữ liệu tạm thời trước khi xử lý hoặc truyền tải.
- Mô tả:
  - Người tham gia: TemporaryStorage, DataCleaning.
- Tiến trình:
  - Dữ liệu thu thập được từ cảm biến được lưu trữ tạm thời trong bộ nhớ.
  - Sau đó, dữ liệu này sẽ được xử lý bởi DataCleaning và ErrorDetection để làm sạch và phát hiện lỗi.
- Kết quả: Dữ liệu được lưu trữ an toàn và có thể truy xuất lại khi cần thiết.

### Biểu đồ kết quả các ca sử dụng:
![Login](https://www.planttext.com/plantuml/png/ZLJ1RjD04Br7oZ-CUk-1j6ah3gZ2792Agg0cWglZM5chphhOkuKUKG-vaXFYW4HQ8GvjHP4uUOKuEEf_x9ymit7YtIIkk3Yoi-_DU_DczZ0JVYhaA6us_40aAMnrKvrFHz1bMdsDe1lf_A_O0Z-3Dw4lM9YU25z42RVEIpw4Rd4rWjcdIAkF4euO_bvoW_8IBj8aza8kmdG9ydH-FOBdH3u_TXBoBAd-VwdLs4YO8FVnx1AVhnxkjRhcGtEyaxn79HUP24VDHhCXip3min35C0c2wVpk30PQ_OGOXOpD9p8ZAZCzxua5UwlL7SJ57mTqNdo3CrPC1P2TCOTOgyzHYMvPwDSItN23vqPgR4ljUJksm5HUO8yu2CH4JhrtqeTpyYqYpahehWNjs5f8t8U5QYCC6TKlc4sq-hAitBRWs3ziH4e5XKcuR8ebeKJjRKPjzBPldJsYr94tzOsyFZfCyAsuXS34tQ_Yxda7b9ixKh2z_Oo2WQTGbwDMDmvP3KKBAPQPafRJIfh5LuFUGRJbHT12e7E1_OzMkb33q4Q6pjhe03FfpgUw1hc7oFz8YfhdR5O9tqNuCVLjFY53xC4ZGxQPerrneENVwBPVJ9FI0h5Y0DybiEAMC_oQJrUDDHlpRRRozEYE89oRfnkbjTHM4XRKxJq4B5cflCwmx_PpXM7mS6_0Dpwf9gdL_BnmTVxWrRvbleHJXXktd582jwm8ry6pYIaQKF6DwIv85rM8ibrI7hWJ-SXs6OhrMuli7OPyO2xwVm00)

## Xác định các phần tử thiết kế
### 1. Các phần tử thiết kế chính
**a. Các thành phần phần cứng (Hardware Components)**

**Cảm biến (Sensors):**

**Chức năng:**
- Thu thập dữ liệu môi trường như nhiệt độ, độ ẩm, áp suất không khí, tốc độ gió.
  
**Ví dụ:**
-  Cảm biến nhiệt độ (Thermometer), cảm biến độ ẩm (Hygrometer), cảm biến áp suất (Barometer).
  
**Bộ xử lý chính (Main Processor):**

**Chức năng:**
- Điều phối hoạt động của hệ thống, xử lý dữ liệu, thực thi các thuật toán phát hiện lỗi.
  
**Bộ nhớ tạm (Temporary Storage):**

**Chức năng:**
- Lưu trữ dữ liệu tạm thời trước khi xử lý hoặc truyền tải.
  
**Nguồn năng lượng (Power System):**

**Chức năng:**
- Cung cấp năng lượng, bao gồm tấm pin mặt trời, tua-bin gió và pin dự trữ.
  
**Hệ thống truyền thông vệ tinh (Satellite Communication Module):**

**Chức năng:**
-Truyền tải dữ liệu từ hệ thống tới trung tâm điều khiển từ xa.

**Mô hình hóa thành phần phần cứng:**

![Diagram](https://www.planttext.com/plantuml/png/V9DBReD038Rtd6AKLRF81LXKKTDANJHI9781bx78g8oDF8O8LJbP5prIhr0DZq0UBIl0zl_vjsT-lhxNGK6qzcLIGVu11Ph5AuWzWg3PiA-Oa3Gip6TYJ5v222P32YpTZ_XuX50BFeF2mp8Tel4hCUPqBjg2evrmZc5UcpEBTGIAMHiKVHHesDaXNFK5dRG5XRdwCZM37jeRsXvznGBIPieIFOt0e3oqskjTI5p21LKSDcTZVzDsV4Jf3KnJONBAqeNUiC6oa-WI5RGEPqX-02dm2LHHsYl_uUWqF-pvXL2ADeF6KR5bYxEqgOiC5ClIAMxO-vfS3kgOjcphSlAl0XIyqtz6yCvS8j3K8BgcqmIo4JoyTkp4ZATXjNgysd5g0f8D9b8ISnMCwJTBIllrX77lQCVY-OJlaIhXnjbO6HFlqluTpqMlfsIDPEED-0K00F__0m00)

**b. Các thành phần phần mềm (Software Components)**

**Bộ xử lý dữ liệu (DataProcessor):**

**Chức năng:**
- Xử lý dữ liệu thô từ các cảm biến, làm sạch dữ liệu và phát hiện các lỗi.
  
**Bộ phát hiện lỗi (ErrorDetectionModule):**

**Chức năng:**
- Phân tích dữ liệu để phát hiện bất thường hoặc lỗi hệ thống.
  
**Quản lý năng lượng (PowerManagementModule):**

**Chức năng:**
- Theo dõi và tối ưu hóa việc sử dụng năng lượng, chuyển hệ thống sang chế độ tiết kiệm năng lượng khi cần thiết.
  
**Quản lý lỗi (FaultManagementModule):**

**Chức năng:**
- Phát hiện và xử lý các lỗi trong hệ thống, kích hoạt cơ chế tự phục hồi (AutoReconfiguration).
  
**Bộ giao tiếp vệ tinh (SatelliteCommunication):**

**Chức năng:**
- Quản lý truyền tải dữ liệu qua vệ tinh tới trung tâm điều khiển.
  
**Hệ thống lưu trữ (StorageModule):**

**Chức năng:**
- Lưu trữ dữ liệu tạm thời hoặc dài hạn, đảm bảo dữ liệu không bị mất khi có sự cố.

  **Mô hình hóa thành phần phần mềm:**
  
  ![Diagram](https://www.planttext.com/plantuml/png/Z5DBJiD03Dtd51QhTi45Pe4gyLc1L54uW9anOKGoZcod5KKz6GkEn1NG9A6q9Qt8Ad7UP_pi-VhudAcXM5jNHOF-5Kk2imK_smg5u9BhXXCbqpDuBm1yXQfmXOPpOK-gB5qzFxuYJFdN9A2XWmKbPSc5gOC1JY5_3uIch_sNijdwNukmN96HjyZfZaDRqVOOcB1wMzEEwfxGrFNqUsfOR4zspYkIEqnOKat93dIviLZ7DNMeHyMI9bC7IuvX0EWgcdzvu5jUzKeSTY6_FZVOLdRK9tHzTHWT6jWvyDJ14tDEUe0BUKxFiMo55czgL8zQBj2eggBH9TTrcwB7dDpMqmIJrj5EXFR7bUAoKyCKikNmkkzgB5ZIGODgBAV6inEfa4caPOyUNOa23hRn_FnYV3_SpxwHGZOkO1oN1SOdv42w6IXG9ce1HrRcb4HCHeBUCdiSazb7vkL0AGM5jWbeb2N-DhyVkklZrlvsKkXRtnGpIY5V-My0003__mC0)
  
  
### 2. Tổ chức các phần tử thiết kế
**Hệ thống được tổ chức theo kiến trúc phân lớp (Layered Architecture), bao gồm các lớp chính:**

**Lớp phần cứng (Hardware Layer):**
- Bao gồm các cảm biến, bộ xử lý chính, nguồn năng lượng và module truyền thông vệ tinh.
  
**Lớp xử lý dữ liệu (Data Processing Layer):**
- Gồm các module xử lý dữ liệu, phát hiện lỗi, và quản lý năng lượng.
  
**Lớp giao tiếp (Communication Layer):**
- Bao gồm các thành phần liên quan đến truyền tải dữ liệu qua vệ tinh.
  
**Lớp lưu trữ (Storage Layer):**
- Quản lý bộ nhớ tạm và dữ liệu lưu trữ dài hạn.

  **Mô hình hóa Kiến trúc phân lớp**
  
  ![Diagram](https://www.planttext.com/plantuml/png/R5BDQiCm3BxxAKJlVO4UHikwiSC2XUm5XArcPh4TP8KGHfziXptINc5uIOgJ-MQaxq-IVxw-Zr6GfNUjwb1_O4EmUyMHc0oSMBzR8Iqzqmu-5S0Tye9i1cI2F-pK1D0jnWWr-HWuArHe_OM3fhYkNy90N8zHoELq56fRA_GOdEkzrIWs-2gOlYK5SCjZd54GPcdhcrAQ12cPFp47FbCQBvTVsi_OjrAXnuOSUIdRhn8MLr6SPIjJI-3qA0YyaUi28uyp9jUUAbao1VFkORz_M0yE1uZaJGJ60GmAAjW04cNhbbWIc29q4uxCGlu7JVnL93Y0CFfu9OuBAxjuCMEN-dStwni5vKjCTiNjBhxEIeHh8a_kDtKaRz97_mK00F__0m00)
  
### 3. Các cơ chế thiết kế được sử dụng
**a. Cơ chế xử lý dữ liệu (Data Processing Mechanism)**
- Dữ liệu từ cảm biến được thu thập, làm sạch và xử lý để đảm bảo tính chính xác.
  
- Xử lý dữ liệu theo chu kỳ, giảm tải cho hệ thống khi năng lượng thấp.

  **Mô hình hóa Cơ chế xử lý dữ liệu**
  
  ![Diagram](https://www.planttext.com/plantuml/png/T94nRiCm301tlOB8L0_vW8OYGzS01Jnq9YH2CM990Kad20g_h4EVr2yKYcKZDX1kedZaKVhx-Js88kiGUtD1TyP0iFj0HVZax4YaIm6Ev4wOEeax-3O0haSHQ2b9vaUYH2IKWQcWRusjj-La0CO5AedQ-8brFM5wa1uLd-76pXxaQxCI609JGALNq1UXdeZR8KRa-qgXrSmOw9ZzqDEY89gh_DHjDRMnSCsThwLCoXrTbrMtWgCnCB_EVl--sTc2KF82Z3Seemni2WgoThIJdS1bdZIHepbGykNd_W400F__0m00)
  
**b. Cơ chế phát hiện lỗi (Error Detection Mechanism)**
- Các thuật toán phân tích dữ liệu được áp dụng để phát hiện bất thường.
  
- Phân biệt lỗi phần cứng (như cảm biến hỏng) và lỗi dữ liệu.

**Mô hình hóa Cơ chế phát hiện lỗi**

![Diagram](https://www.planttext.com/plantuml/png/R951JiCm44NtFiMegsJH2tY1kYZi8Y5wWY7-b0Z74tcSIe1wCXOSYIiWEo4YLRomv3ypx-kFVxw-3veufh7tPk3sZS-WtNsC4kc8X3Pr4gX1-ygXqtv7duQezQnAHqxy6AM5giIYvpDCIYvMZXDREY6en2pKbkO1kFmsHDS5LpmNoqRSwB5GER1__y0_wWfKssdy2OF4jC8-yEXJmu7Fw17I3TSLlzAZLIpJArHj9y3S7g7YBoXIzPBlkLvRUXRnu53C3TriPx-_smveyy8kdOF-RGwESa93smEPj9t9aY8u9PJFcyAekPe3Wik_-mi00F__0m00)

**c. Cơ chế quản lý năng lượng (Power Management Mechanism)**
- Theo dõi mức năng lượng và tự động chuyển đổi chế độ hoạt động (tiết kiệm năng lượng khi pin yếu).
  
- Ưu tiên cung cấp năng lượng cho các thành phần thiết yếu.

  **Mô hình hóa Cơ chế quản lý năng lượng**
  
  ![Diagram](https://www.planttext.com/plantuml/png/Z9112i9034NtFKNeIXTUe0iHroq8wW529zJ1pgHCqXOLJ-R28ta5wLYqBWIpJ5x-_ydZTb-9Oj3MrKc3vH4hWdJ3FGKeq6D5Zhn2GUK1lHMNmYK1A6iKWKXjJwBaOdSenzugXpZAgQDwDiz6K55R6R4mw8MArgXAuJH07LipJgMtMXvsd7CVLmisD46ktma-CGisRKtlBDoeTVPCaTeBLbEHltmI-3foiLZ-iCn0o1k19ZvENgTUanLvCpps2G00__y30000)
  
**d. Cơ chế tự phục hồi (Auto-Reconfiguration Mechanism)**
- Khi lỗi được phát hiện, hệ thống sẽ tự động tái cấu hình để tiếp tục hoạt động.
  
**Ví dụ:**
- Ngắt cảm biến bị lỗi và sử dụng các cảm biến dự phòng nếu có.

**Mô hình hóa Cơ chế tự phục hồi**

![Diagram](https://www.planttext.com/plantuml/png/b591JWCn3Bpd5LPFkuT-80TKKE5M2RKlC8ctHCqcLUnKAgWluy2J-09AThjIqO94RixOCvv9lZu-LooO9FTU7T4SS4-mkCyIbrioCNHkdnEAYm4sP5unEEuNyAu0Z4TcUCBiPOC1zzHJa4sqsLF5ox4aPAJsS9Fe69DeU4mffcqjMZqGZErfKgJTcONwfYlesDHgE4Ld5S1bajzHu9WclPwGSw8r2ZQj7j5INVTnZ2-UcZcg1pI7VFmd8Hfn9vHvncfqNIDmCVo81WFwyzl0R55GmtEAXfZ9bhls9gTAg-2Nj9VBksiGUeoSeIRtvyYDOJrPON0TzEW2y01rw3mhcBTJYEObT9ct35J6O7XyLXUrec3BP_i6003__mC0)
  
**e. Cơ chế truyền thông (Communication Mechanism)**
- Dữ liệu được truyền qua vệ tinh theo lô để tiết kiệm năng lượng.
  
- Hỗ trợ truyền dữ liệu ưu tiên cao (báo cáo lỗi) khi có sự cố khẩn cấp.

  **Mô hình hóa Cơ chế truyền thông**
  
  ![Diagram](https://www.planttext.com/plantuml/png/Z911Qa9138RtSuhWIXTUu2sAKEdkGMbFy3iJxT2PZ4potCWxcGkFv1NAFEI92w5PXV0bNvBRvRfHGxKX9tU4_yM1QV5USXuaUbWiGZtx7qZKlA2p8_89glGDuvIYyJFRW1PM8PgZRM5O1XWw-gp5iog7Lbjrj2ibCUJUKDbpF4tJ866vwkYUEg9njdvWIDP3SE3COdq9G-9P6jZOsyJelwJA4YRyYu-bMhC-WD4vUY5ShzzUFQ2RJrVQjsPgYxZHRLX2U_8V0000__y30000)
  
**f. Cơ chế lưu trữ (Storage Mechanism)**
- Dữ liệu được lưu trữ tạm thời nếu kết nối vệ tinh bị gián đoạn.
  
- Cơ chế nén dữ liệu được áp dụng để tối ưu hóa bộ nhớ.

****Mô hình hóa Cơ chế lưu trữ**

![Diagram](https://www.planttext.com/plantuml/png/j90n2i9044NxESMGoXIvG0f9OHiGz0B3xgZ191jc9e4GSZ8BZ-GLP3LQnDgfFfy7Zp-FsxrG8x6-gQ4ZTwKpOtAm836Kx2xKLjeaE06YgqaLZznqGKZ63pK1lauj2E_8QEF9ACUz1CUgx6ENvZY4oY-ei4d5mvjELoWWpb_R8Yc3x-i_gG1_DsNPTgNEqOHQFR4eHYdCK73huz-U0000__y30000)

### Giải thích biểu đồ:
- Hệ thống trạm thời tiết giao tiếp trực tiếp với hệ thống quản lý dữ liệu **(IDataManagement)** để truyền dữ liệu thời tiết.
- Hệ thống bảo trì sử dụng **IMaintenance** để giám sát, bảo trì, và cập nhật các trạm thời tiết từ xa.
- Hệ thống giao tiếp vệ tinh **(ICommunication)** là trung gian truyền dữ liệu giữa các hệ thống trạm và hệ thống quản lý/lưu trữ.
- Hệ thống dự báo thời tiết sử dụng dữ liệu từ hệ thống quản lý và cung cấp dự báo thời tiết qua **IForecasting.**
