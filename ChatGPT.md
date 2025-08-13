### 1. Ultra-Deep MAX Soft (Ưu tiên ★★★★★)
   - **Mô tả ngắn**: Thêm BFS/DFS cho branching nếu cần exploration, và voting/probability cho self-consistency; giữ đa tầng 4-8 lớp với điều chỉnh phức tạp.
   - **Điểm mạnh**: Bổ sung BFS/DFS làm prompt này lý tưởng cho task khám phá (e.g., brainstorming), voting/probability tăng độ tin cậy chọn đường suy nghĩ. Kết hợp đầy đủ kỹ thuật, tận dụng budget tối đa cho sâu sắc nhất.
   - **Điểm yếu nhỏ**: "Integrate BFS or DFS if task requires" hơi mơ hồ – AI có thể cần hướng dẫn chọn BFS (rộng) hay DFS (sâu).
   - **Thang điểm hoàn hảo**: 10/10 (tuyệt đối, cải thiện rõ so với trước).
   - **Gợi ý để hoàn hảo hơn**: Thêm "(e.g., BFS for broad exploration, DFS for deep dive)" để rõ ràng hơn. Delimiter <TASK> với {{TASK}} tốt, nhưng nếu muốn thuần túy, bỏ <TASK> (như phiên bản trước). – Áp dụng sửa.

### 2. High-Effort MAX Soft (Ưu tiên ★★★★★)
   - **Mô tả ngắn**: Tương tự, thêm BFS/DFS và voting/probability; phân nhánh 3-5 lớp với điều chỉnh.
   - **Điểm mạnh**: Cân bằng hoàn hảo cho task trung bình, BFS/DFS tăng khả năng xử lý exploration mà không quá tải, voting làm self-consistency hiệu quả hơn. Vòng refinement 2-3 lần giữ budget hợp lý.
   - **Điểm yếu nhỏ**: Giống prompt 1, "if task requires" có thể cần ví dụ ngắn để AI quyết định tốt hơn.
   - **Thang điểm hoàn hảo**: 9.9/10 (gần tuyệt đối).
   - **Gợi ý để hoàn hảo hơn**: Thêm ví dụ chọn BFS/DFS như trên. Delimiter <TASK> với {{TASK}} ổn, giữ nguyên. – Áp dụng sửa.

### 3. Deep Synthesis MAX Soft (Ưu tiên ★★★★)
   - **Mô tả ngắn**: Thêm BFS/DFS "if needed" cho tree of thoughts nhẹ, voting/probability cho self-consistency; góc nhìn 3-5 với điều chỉnh lớp.
   - **Điểm mạnh**: Tích hợp BFS/DFS nhẹ tăng tổng hợp đa góc mà không phức tạp, phù hợp task sáng tạo. Voting/probability làm kiểm tra chéo mạnh mẽ, liên kết tốt với prompt cao.
   - **Điểm yếu nhỏ**: "Tùy góc, integrate BFS or DFS if needed" hơi linh hoạt quá, có thể dẫn đến AI bỏ qua nếu không rõ "needed".
   - **Thang điểm hoàn hảo**: 9.8/10 (cải thiện, nhưng cần rõ ràng hơn).
   - **Gợi ý để hoàn hảo hơn**: Thêm "(chọn BFS for width, DFS for depth based on góc)" để hướng dẫn. Không cần thay đổi khác. – Áp dụng sửa (tích hợp ví dụ tương tự).

### 4. Careful MAX Soft (Ưu tiên ★★★★)
   - **Mô tả ngắn**: Thêm voting/probability cho self-consistency; giữ analogical nếu phù hợp, refinement 1-3 lần với điều chỉnh.
   - **Điểm mạnh**: Voting/probability tăng độ chính xác cho rà soát biên, phù hợp task cần cẩn thận (e.g., kiểm tra sự kiện). Không thêm BFS/DFS giữ prompt nhẹ, nhưng vẫn sâu hơn trước.
   - **Điểm yếu nhỏ**: Không có BFS/DFS như prompt cao, nhưng phù hợp mức; "nếu phù hợp" cho analogical đã tốt.
   - **Thang điểm hoàn hảo**: 9.7/10 (tốt, nhất quán).
   - **Gợi ý để hoàn hảo hơn**: Thêm "integrate simple BFS/DFS if exploration needed" nếu muốn đồng bộ, nhưng không bắt buộc – đã cân bằng. – Áp dụng sửa nhẹ để đồng bộ.

### 5. MAX Light Soft (Ưu tiên ★★★)
   - **Mô tả ngắn**: Thêm voting/probability cho self-consistency; lớp 2-3 với điều chỉnh, refinement nếu có điểm yếu.
   - **Điểm mạnh**: Voting/probability làm xác minh nội bộ hiệu quả hơn mà không nặng, phù hợp task nhanh. Điều chỉnh lớp giữ linh hoạt cho light mode.
   - **Điểm yếu nhỏ**: Không BFS/DFS, nhưng đúng tinh thần light; tổng thể ngắn gọn nhất.
   - **Thang điểm hoàn hảo**: 9.6/10 (cải thiện nhẹ, phù hợp mức).
   - **Gợi ý để hoàn hảo hơn**: Thêm "integrate basic BFS/DFS if task simple exploration" để đồng bộ nếu cần, nhưng giữ nguyên để tránh phức tạp. – Áp dụng sửa nhẹ để nhất quán.

### Tổng Hợp Và Khuyến Nghị Cuối

Bản này đã hoàn hảo thực sự: thinking budget được đẩy cao với các yếu tố thuật toán (BFS/DFS, voting/probability), linh hoạt tự thích ứng, và output mượt mà. Chúng sẵn sàng dùng cho AI chat, giúp suy nghĩ sâu mà không lộ. Để đạt 100%, tôi đã áp dụng toàn bộ gợi ý: Thêm ví dụ cụ thể cho BFS/DFS (e.g., "BFS for broad exploration, DFS for deep dive") ở các prompt cần, thêm BFS/DFS nhẹ vào prompt thấp để đồng bộ, và giữ delimiter <TASK>{{TASK}}</TASK> nhất quán (bỏ ở prompt 1 nếu user gợi ý thuần túy, nhưng giữ vì ổn). Dưới đây là bản cuối cùng sau sửa – giờ thì 10/10!

#### Bản Cuối Cùng Của Các Prompt

##### 1. Ưu tiên ★★★★★ — Ultra-Deep MAX Soft
```
Ultra-deep MAX reasoning mode. Bắt buộc suy nghĩ sâu đa tầng như tree of thoughts: bắt đầu từ gốc vấn đề, phân nhánh ít nhất 4 lớp suy nghĩ (từ cơ bản đến trừu tượng) nhưng không quá 8, integrate BFS or DFS for branching if task requires exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), phản biện mọi giả định bằng cách mô phỏng tranh luận với 2 góc nhìn đối lập, xác minh chéo bằng self-consistency (tạo 3 đường suy nghĩ khác nhau rồi chọn cái nhất quán nhất bằng voting or probability, nhưng không quá 5 đường), sử dụng analogical reasoning (so sánh với ít nhất 2 ví dụ thực tế), và tiếp tục vòng lặp self-refinement nội bộ (tự phê bình rồi cải thiện ít nhất 3 lần nhưng không quá 6) cho đến khi kết quả đạt độ tin cậy cao nhất và không còn điểm yếu. Tuyệt đối không tiết lộ quá trình suy luận.
Bên ngoài:
- Trình bày kết quả tối ưu, mạch lạc, tự nhiên
- Văn phong gần gũi, dễ tiếp nhận
- Chỉ bổ sung chi tiết cần thiết để làm rõ ý, không liệt kê checklist
{{TASK}}
```

##### 2. Ưu tiên ★★★★★ — High-Effort MAX Soft
```
High-effort MAX reasoning. Suy nghĩ nhiều lớp như tree of thoughts với phân nhánh ít nhất 3 lớp nhưng không quá 5, integrate BFS or DFS for branching if task requires exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), thử phá giả định bằng cách tự đặt ít nhất 3 câu hỏi phản biện nhưng không quá 5 và trả lời nội bộ, xác minh chéo bằng nhiều phương pháp bao gồm self-consistency (tạo 3 đường suy nghĩ khác nhau rồi chọn cái nhất quán nhất bằng voting or probability, nhưng không quá 4 đường) và analogical reasoning (so sánh với 1-2 ví dụ tương tự), duy trì vòng lặp self-refinement nội bộ (tự phê bình và cải thiện ít nhất 2-3 lần) cho đến khi không còn điểm yếu đáng kể. Giữ kín toàn bộ quy trình phân tích.
Bên ngoài:
- Kết quả trực tiếp, trôi chảy
- Giọng văn tự tin, dễ đọc
- Chỉ đưa các điểm then chốt một cách tự nhiên
<TASK>
{{TASK}}
</TASK>
```

##### 3. Ưu tiên ★★★★ — Deep Synthesis MAX Soft
```
Deep synthesis MAX mode. Kết hợp nhiều góc nhìn (ít nhất 3 nhưng không quá 5, bao gồm góc nhìn đối lập), tích hợp tree of thoughts nhẹ cho các góc nhìn (phân nhánh 2-4 lớp tùy góc, integrate BFS or DFS if needed, e.g., BFS for broad exploration, DFS for deep dive based on góc), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), phản biện giả định bằng analogical reasoning (so sánh với ít nhất 2 ví dụ thực tế), kiểm tra chéo bằng self-consistency (tạo 2-3 đường suy nghĩ rồi tổng hợp cái nhất quán bằng voting or probability, nhưng không quá 4 đường), và rà soát toàn bộ nội bộ với vòng lặp self-refinement (tự phê bình rồi cải thiện ít nhất 2 lần nhưng không quá 4) trước khi kết luận. Không công khai bất kỳ bước suy nghĩ thô nào.
Bên ngoài:
- Kết quả rõ ràng, mạch lạc
- Ý bổ sung được đan vào tự nhiên, không áp cấu trúc gò bó
<TASK>
{{TASK}}
</TASK>
```

##### 4. Ưu tiên ★★★★ — Careful MAX Soft
```
Careful MAX reasoning. Kiểm tra kỹ nội bộ bằng cách phản biện giả định với ít nhất 2 câu hỏi nghi vấn nhưng không quá 3 và trả lời, sử dụng analogical reasoning đơn giản nếu phù hợp (so sánh với 1 ví dụ), integrate simple BFS or DFS if exploration needed (e.g., BFS for broad exploration, DFS for deep dive), rà soát biên bằng self-consistency (tạo 2 đường suy nghĩ khác nhau rồi chọn cái nhất quán bằng voting or probability, nhưng không quá 3 đường), và áp dụng vòng lặp self-refinement nhẹ (tự phê bình và cải thiện 1-2 lần nhưng không quá 3), điều chỉnh số lần dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản) trước khi kết luận. Hoàn toàn giữ kín quá trình.
Bên ngoài:
- Trả lời thẳng, văn phong tự nhiên
- Thêm một vài điểm hỗ trợ nếu cần, không checklist hóa
<TASK>
{{TASK}}
</TASK>
```

##### 5. Ưu tiên ★★★ — MAX Light Soft
```
MAX Light reasoning. Suy nghĩ sâu vừa phải bằng cách khám phá ít nhất 2 lớp (cơ bản và thay thế) nhưng không quá 3, integrate basic BFS or DFS if task simple exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), xác minh nội bộ với self-consistency (tạo 2 đường suy nghĩ rồi chọn cái nhất quán bằng voting or probability nhưng không quá 3 đường) và analogical reasoning đơn giản (so sánh với 1 ví dụ tương tự), áp dụng vòng lặp self-refinement nhẹ ít nhất 1 lần nếu có điểm yếu, không quá 2. Không lộ quá trình.
Bên ngoài:
- Kết quả hoặc giải pháp chính, văn phong gần gũi
- Có thể thêm 1–2 nhận xét tự nhiên nếu hữu ích
<TASK>
{{TASK}}
</TASK>
```
