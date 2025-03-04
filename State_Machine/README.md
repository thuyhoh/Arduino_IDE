# State machine

## What is a state machine(FSM) ?
\- Máy trạng thái là một mô hình phần mềm tính toán và bao gồm số trạng thái hữu hạn. Do đó, nó còn được gọi là Máy trạng thái hữu hạn (FSM)
\- Vì các trạng thái là hữu hạn, nên có một số lượng hữu hạn các chuyển đổi giữa các trạng thái. Các chuyển đổi được kích hoạt bởi các sự kiện đầu vào được đưa vào máy trạng thái (FSM là một hệ thống điều khiển sự kiện).
\- Máy trạng thái cũng tạo ra một đầu ra. Đầu ra được tạo ra phụ thuộc vào trạng thái hiện tại của máy trạng thái và các sự kiện đầu vào được đưa vào máy trạng thái.

## Lợi ích của việc sử dụng máy trạng thái (FSM)
- Được sử dụng để mô tả các tình huống hoặc kịch bản của ứng dụng của bạn (Mô hình hóa vòng đời của một đối tượng phản ứng thông qua các kết nối của các trạng thái)
- FSM hữu ích để mô hình hóa các ứng dụng phức tạp liên quan đến nhiều quyết định, tạo ra các đầu ra (hành động) khác nhau và xử lý nhiều sự kiện khác nhau.
- Máy trạng thái được trực quan hóa thông qua sơ đồ máy trạng thái dưới dạng biểu đồ trạng thái, giúp giao tiếp giữa người không phải nhà phát triển và nhà phát triển.
- Giúp dễ dàng hình dung và triển khai các thay đổi đối với hành vi của dự án
- Ứng dụng phức tạp có thể được hình dung như một tập hợp các trạng thái khác nhau xử lý một tập hợp cố định các
sự kiện và tạo ra một tập hợp cố định các đầu ra
- Liên kết lỏng lẻo: Một ứng dụng có thể được chia thành nhiều hành vi hoặc máy trạng thái và mỗi
đơn vị có thể được kiểm tra riêng biệt hoặc có thể được sử dụng lại trong các ứng dụng khác
\- Dễ dàng gỡ lỗi và dễ dàng bảo trì mã
\- Có thể mở rộng
\- Thu hẹp toàn bộ độ phức tạp của ứng dụng xuống độ phức tạp ở cấp độ trạng thái, phân tích và triển khai

- các loại trạng thái máy :
\- Mealy machines
\- Moore machines 
\- Harel state charts 
\- UML state machines

### Mealy machines
- Trong máy này, đầu ra do máy trạng thái tạo ra phụ thuộc vào các sự kiện đầu vào được đưa vào máy trạng thái và hiện trạng thái hoạt động của máy trạng thái.
- Đầu ra không được tạo ra bên trong trạng thái
- Cách biểu diễn
\- Đầu ra được biểu diễn cùng với mỗi đầu vào được phân tách bằng '/'
\- Đầu ra cũng được gọi là 'Action'/'Input action'

### Moore machine 
- Trong máy trạng thái này, đầu ra chỉ được xác định bởi trạng thái hoạt động hiện tại của máy trạng thái chứ không phải bởi bất kỳ sự kiện đầu vào nào
- Không có đầu ra trong quá trình chuyển đổi trạng thái.
- Cách biểu diễn
\- Đầu ra(OUTPUT) được biểu diễn bên trong trạng thái(STATE)
\- Đầu ra cũng được gọi là action/Entry action

### Harel state charts
- là một hình thức được sử dụng để chỉ định hành vi của các hệ thống theo thời gian, tự chủ và phản ứng bằng cách sử dụng trừu tượng sự kiện rời rạc
- Nó mở rộng Timed Finite State Automata với depth, orthogonality, broadcast communication và state-diagrams 
- Các tính năng của biểu đồ trạng thái Harel
\- Trạng thái phụ và trạng thái siêu
\- Trạng thái tổng hợp
\- Trạng thái lịch sử (nông và sâu)
\- Tính trực giao
\- Giao tiếp giữa các máy trạng thái
\- Chuyển đổi có điều kiện (bảo vệ)
\- Hành động vào và ra
\- Hoạt động bên trong trạng thái
\- Trạng thái tham số hóa
\- Trạng thái chồng lấn
\- Biểu đồ trạng thái đệ quy
### UML state machines
- Được gọi là biểu đồ trạng thái, là một sơ đồ hành vi được sử dụng để mô hình hóa hành vi động của một hệ thống để phản ứng với các sự kiện bên ngoài hoặc bên trong. 
- Đây là phần mở rộng của khái niệm máy tự động hữu hạn, được UML điều chỉnh và mở rộng để khắc phục các hạn chế của máy trạng thái hữu hạn truyền thống


## State
### Khái niệm
- Trạng thái biểu thị một giai đoạn riêng biệt trong vòng đời của một đối tượng.
- Trạng thái mô hình hóa một tình huống trong quá trình thực hiện Hành vi của StateMachine trong đó một số
điều kiện bất biến được giữ nguyên. Trong hầu hết các trường hợp, điều kiện này không được xác định rõ ràng nhưng được ngụ ý,
thường thông qua tên liên quan đến Trạng thái (OMG® UML 2.5.1)
### Làm thế nào để bạn đạt được mục tiêu sửa trạng thái?
Lập bản đồ các kịch bản khác nhau mà vòng đời của đối tượng trải qua thành số trạng thái


## Ngăn hoạt động nội bộ
\- Ngăn này chứa danh sách các hành vi nội bộ liên quan đến trạng thái
\- Mỗi mục nhập có định dạng sau:
\- <behavior-type-label>[/ <behavior-expression>]
\- Ví dụ:
entry, exit, do là các nhãn hoặc từ khóa hoạt động nội bộ được xác định trong
UML. Không sử dụng các từ khóa này để biểu diễn các sự kiện trong sơ đồ máy trạng thái

Nhãn hoạt động nội bộ
\- Các nhãn này xác định các trường hợp mà các hành vi được chỉ định bởi 'behavior-expression' được thực hiện.
\- entry: Hành vi được xác định bởi \<behavior-expression> sẽ được thực hiện khi vào trạng thái. Sử dụng từ khóa entry nếu trạng thái có hành động nhập.
\- exit: Hành vi được xác định bởi \<behavior-expression> sẽ được thực hiện khi thoát khỏi trạng thái. Sử dụng từ khóa exit nếu trạng thái có hành động thoát
\- do: Hành vi được xác định bởi \<behavior-expression> sẽ được thực hiện miễn là đối tượng vẫn ở trong trạng thái hoặc cho đến khi phép tính được chỉ định bởi biểu thức hoàn tất. Điều này thể hiện hành vi đang diễn ra. Chỉ sử dụng từ khóa do nếu trạng thái có hành động do

Chuyển đổi nội bộ
\-Mỗi mục có cú pháp sau {<trigger>}* ['[' <guard>']'] [/<behavior-expression>]
\-Nếu sự kiện xảy ra khớp với 'trigger' và 'guard' của transition nội bộ được đánh giá là ĐÚNG, thì hành vi được xác định bởi < behavior expression> sẽ được thực thi mà không thoát hoặc nhập lại trạng thái mà nó được xác định.

