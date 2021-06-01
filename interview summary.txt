Thông thường 1 buổi phỏng vấn sẽ có 5 phần:
	1. Hỏi về bản thân
	2. Hỏi về ngôn ngữ
	3. Hỏi thuật toán
	4. Đặt câu hỏi
Ngoài ra, sẽ có hỏi những câu hỏi về tech, DSA, ... xen kẽ trong lúc phỏng vấn.

1. Hỏi về bản thân:
	Những câu hỏi thường gặp:
	- Giới thiệu bản thân
	- Kinh nghiệm
	- Công việc trước đó: làm vị trí gì, làm thứ gì, nhiệm vụ (task) cụ thể là làm gì, lý do nghỉ việc
	- Project cũ: giới thiệu, làm gì, công nghệ gì, có gì trong đó...
	- Điểm mạnh/yếu
	- Hỏi xoáy vào những thứ trong CV
	- Sở thích, thích chơi điện tử thì chơi game gì, rank gì, mmr bao nhiêu
	- Em thường update công nghệ ở blog nào.
	- Em có quan tâm công nghệ nào ko?
	- [Hot] Kể về một task khó khăn nhất của em và cách em giải quyết
		https://tuoitre.vn/chi-1-cau-hoi-elon-musk-biet-ai-la-nguoi-tai-ai-chem-gio-do-la-cau-gi-20210127133103409.htm
	- 
2. Hỏi về kiến thức tech tổng hợp:
	Những câu hỏi thường gặp:
	- Scrum:
		+ Agile là gì? Scrum là gì?
		+ Scrum có ưu điểm gì?
		+ Scrum hơn waterfall chỗ nào?
		+ Tại sao phải dùng Scrum?
		+ Scrum giải quyết được vấn đề gì?
		+ ...
	- OOP:
		+ 4 tính chất
		+ Design pattern
		+ Abstract class vs Interface
		+ Static là gì
		+ class vs instance
		+ class vs structure
		+ overloading vs overriding
		Example resource:	https://www.edureka.co/blog/interview-questions/oops-interview-questions/
							https://career.guru99.com/top-50-oops-interview-questions/
	- Web:
		+ Browser:
			~ URL dài tối đa bao nhiêu ký tự
			~ Session vs Cookie
			~ Local Storage vs Session Storage vs Web SQL vs Cookies
			~ RestAPI:
				- GET POST cái nào bảo mật hơn? Cái nào gửi được data cho server?
				- Tại sao phải sinh ra GET POST PUT DELETE? Dùng POST để get/delete/update được không? Nếu được thì tại sao phải chia ra riêng các method?
					Ví dụ: tại sao không dùng thế này?
						POST /users/get/:id
						POST /users/get
						POST /users/create
						POST /users/update
						POST /users/delete
				- 
			~ 
		+ Mạng:
			- 7 tầng OSI
			- So sánh TCP vs UDP? Videocall dùng cái nào?
	- Microservice:
		+ Là gì?
		+ Công dụng?
	- Version Control: git, svn
		+ Pull Request là gì
		+ Process khi làm việc với git: khi nhận 1 task mới cần làm gì cho đến khi xong task?
 	- 
	- 
3. Hỏi về ngôn ngữ/framework:
	Hỏi cụ thể về kiến thức ngôn ngữ, đào sâu vào ngôn ngữ/framework.
	1 vài câu hỏi:
		JS/NodeJS/React/Redux:
			- 
		Java:
			- 
		Chung:
			- So sánh foreach vs map vs reduce vs filter
			- Tạo quá nhiều thread trong 1 process thì có hại gì ko? Vì sao?
			- Pass by reference vs Pass by value là gì? Ngôn ngữ X là pass by gì
	Hỏi về database:
		SQL:
			-
			-
		NoSQL (Mongo, ...):
			-
			-
4. Hỏi thuật toán:
	Thuật toán:
		1. Cho 1 mảng. Tìm max(a[j] - a[i]) với i <= j
			VD: [7,1,2,4,3,6,5] => 6 - 1 = 5
				[7,6,4,3,2] => 0
			ĐA: time: 1 for, space: O(1)
		2. Cho 1 mảng, trả về mảng đó có thể chia thành 3 phần có tổng = nhau ko
			VD: [9,4,5,3,6] => true: [9], [4,5], [3,6]
				[9,6,5,4,3] => false
			ĐA: time: 1 for, space: O(1)
		3. Cho 1 mảng. Move giá trị 0 xuống cuối mảng
			VD: [0, 1, 0, 0, 3, 12] => [1, 3, 12, 0, 0]
			Yêu cầu: các số khác 0 giữ nguyên thứ tự. Không dùng mảng phụ.
		4. Cho 1 mảng, trả về dãy tăng liên tiếp lớn nhất có độ dài = mấy
			VD: [10, 1, 100, 3, 9, 2, 99, 8, 4, 7] => 4 (1, 2, 3, 4)
		5. Cho mảng, tìm số nguyên dương lớn nhất ko thuộc mảng.
		6. Cho mảng, tìm 2 số trùng nhau.
		7. Cho mảng và 1 số, tìm 2 số trong mảng tổng = số cho trước.
		8. Cho mảng, tìm số lớn thứ 2.
			=> chỉ dùng 1 for
		9. Tìm phần tử lớn thử k trong mảng (ko đc sort)
		Tip: Thông thường có 2 cách để giảm độ phức tạp:
				1. Giảm từ O(n2) -> O(n log n): dùng sort O(n log n)
				2. Giảm bớt 1 n: dùng hash. Insert/get/delete: O(1), Space: O(n)
			Thông thường những bài thuật toán như này thì yêu cầu của người phỏng vấn muốn là nghe 1 solution nào đó (có thể rất tệ vd O(n2), vét cạn, ...), sau đó người phỏng vấn sẽ gợi ý để optimize dần dần để ra được best solution. Vì thế khi đọc được đề thì nghĩ được solution nào thì cứ nói ra. Sau đó mới bắt đầu nghĩ về các solution optimize hơn (có thể tham khảo 2 cách giảm độ phức tạp trên). vì khi ấy kể cả khi mình không nghĩ ra solution optimize thì ít nhất mình cũng đã nêu được 1 solution nào đó và cũng đã có cố gắng optimize.
	DSA:
		1. Find longest common substring: https://www.geeksforgeeks.org/longest-common-substring-dp-29/
		2. Mảng vs linked list, ưu nhược
		3. map vs hash table khác nhau gì
		4. Stack vs queue? Cái nào hay dùng hơn?
		5. Hashmap implement như nào
		6. Order hashmap implement như nào

	IQ:
		- Cho 8 đồng xu và cân thăng bằng trong đó 1 xu nặng/nhẹ hơn. Tìm xu giả.
		ĐA: 2 lần cân
		- Cho 8 đồng xu và cân thăng bằng trong đó 1 xu giả không biết nặng nhẹ. Tìm xu giả.
		ĐA: 3 lần cân
		- Đồng hồ đang chỉ 5:45, lần tiếp theo 2 kim trùng nhau là khi nào



chưa có gì ở đây hết