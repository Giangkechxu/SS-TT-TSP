Dự án này triển khai và so sánh hiệu suất của 4 thuật toán khác nhau để giải bài toán Traveling Salesman Problem (TSP): Tìm đường đi ngắn nhất đi qua tất cả các thành phố và quay trở lại điểm xuất phát.
Các thuật toán triển khai:
    1. Branch and Bound (B&B - Nhánh và Cận)
        + Loại: Thuật toán chính xác (Exact Algorithm).
        + Đặc điểm: Sử dụng cây không gian trạng thái và các giá trị biên (bound) để loại bỏ các nhánh không tiềm năng.
        + Ưu điểm: Luôn tìm ra lời giải tối ưu nhất.
        + Nhược điểm: Độ phức tạp thời gian tăng theo hàm mũ $O(n^2 \cdot 2^n)$, chỉ hiệu quả với số lượng thành phố nhỏ.
    2. Genetic Algorithm (GA - Giải thuật Di truyền)
        + Loại: Meta-heuristic (Dựa trên tiến hóa tự nhiên).
        + Cơ chế: Quần thể, Chọn lọc, Lai ghép (Crossover) và Đột biến (Mutation).
        + Phù hợp: Không gian tìm kiếm lớn, cần tìm lời giải "đủ tốt" trong thời gian nhanh.
    3. Ant Colony Optimization (ACO - Tối ưu hóa Đàn kiến)
        + Loại: Meta-heuristic (Dựa trên hành vi bầy đàn).
        + Cơ chế: Sử dụng "vết pheromone" để đánh dấu các con đường ngắn. Theo thời gian, các đường đi ngắn nhất sẽ tích lũy nồng độ pheromone cao hơn.
        + Ưu điểm: Rất mạnh trong việc tìm kiếm các cấu trúc đường đi trong đồ thị.
    4. Simulated Annealing (SA - Mô phỏng luyện kim)
        + Loại: Meta-heuristic (Dựa trên quá trình nhiệt luyện kim loại).
        + Cơ chế: Chấp nhận các lời giải tệ hơn với một xác suất nhất định (theo hàm Gibbs) để thoát khỏi tối ưu địa phương (local optimum).
        + Đặc điểm: Đơn giản để triển khai nhưng cần tinh chỉnh tham số nhiệt độ T kỹ lưỡng.