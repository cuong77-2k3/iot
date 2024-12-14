<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đồ án IOT - Bãi Đỗ Xe</title>
    <script src="https://www.gstatic.com/firebasejs/8.10.0/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/8.10.0/firebase-database.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
    <style>
        /* Cập nhật phong cách phần tiêu đề */
        .header-section {
            background-color: #0177A9;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 24px;
            border-bottom: 5px solid #0177A9;
        }

        .header-description {
            font-size: 16px;
            font-weight: bold;
            margin-top: 10px;
        }

        /* Hiệu ứng hover cho nút */
        .btn:hover {
            transform: scale(1.1);
            transition: all 0.3s ease-in-out;
        }

        /* Viền màu xanh cho phần giới thiệu */
        .intro-section {
            border: 2px solid #007bff;
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 30px;
            background-color: #f9f9f9;
        }

        /* Thông tin liên hệ ở dưới cùng */
        .contact-info {
            background-color: #f8f9fa;
            padding: 20px;
            border-top: 2px solid #007bff;
            text-align: center;
            margin-top: 40px;
        }

        .contact-info h4 {
            margin-bottom: 15px;
        }

        .contact-info p {
            margin-bottom: 10px;
        }

        /* Hiệu ứng cho các bảng */
        table {
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        /* Nền màu xanh dương cho nút chuyển trang */
        .btn-info {
            background-color: #007bff;
            border: none;
        }

        .btn-info:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container mt-5">
        <!-- Tiêu đề với nền xanh dương -->
        <div class="header-section">
            <h1>Đồ án IOT - Bãi Đỗ Xe Thông Minh</h1>
            <p class="header-description">Hệ thống tự động theo dõi biển số xe và thời gian vào/ra</p>
        </div>

        <div class="d-flex justify-content-center mt-4">
            <img src="b.jpg" alt="Hình ảnh bãi đỗ xe" class="img-fluid rounded" style="max-width: 25%; border: 2px solid #007bff;">
        </div>

        <div class="d-flex justify-content-around text-center mt-4 mb-5">
            <div>
                <h5>Số lượng xe hiện tại</h5>
                <p id="current-car-count" class="fw-bold">0</p>
            </div>
            <div>
                <h5>Vị trí còn trống</h5>
                <p id="available-spots" class="fw-bold">0</p>
            </div>
        </div>

        <h2 class="text-center mt-5">Thông Tin Xe</h2>
        <div class="table-responsive">
            <table class="table table-bordered text-center">
                <thead class="table-light">
                    <tr>
                        <th colspan="3">Xe Vào</th>
                        <th colspan="3">Xe Ra</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td id="in-license-plate">Biển số vào</td>
                        <td id="in-date">Ngày vào</td>
                        <td id="in-time">Thời gian vào</td>
                        <td id="out-license-plate">Biển số ra</td>
                        <td id="out-date">Ngày ra</td>
                        <td id="out-time">Thời gian ra</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="d-flex justify-content-around mt-4">
            <button class="btn btn-primary" id="open-gate-in">Mở Cửa Vào</button>
            <button class="btn btn-danger" id="open-gate-out">Mở Cửa Ra</button>
        </div>

        <h2 class="text-center mt-5">Danh Sách Xe</h2>
        <div class="table-responsive">
            <table class="table table-bordered text-center">
                <thead class="table-dark">
                    <tr>
                        <th>Số Thứ Tự</th>
                        <th>Biển Số Xe</th>
                        <th>Thời Gian Vào</th>
                        <th>Thời Gian Ra</th>
                    </tr>
                </thead>
                <tbody id="car-list">
                </tbody>
            </table>
        </div>

        <div class="text-center mt-4">
            <p>Giám sát dữ liệu: <a href="http://surl.li/lczsue" target="_blank">http://surl.li/lczsue</a></p>
        </div>
        
        <!-- Button to switch to web2 -->
        <div class="text-center mt-4">
            <button class="btn btn-info" id="switch-to-web2">Chuyển sang Web 2</button>
        </div>

        <div class="d-flex justify-content-center mt-4">
            <img src="a.png" alt="Hình ảnh bãi đỗ xe" class="img-fluid rounded" style="max-width: 40%; border: 2px solid #007bff;">
        </div>

        <!-- Thông tin liên hệ -->
        <div class="contact-info">
            <h4>Liên Hệ Với Chúng Tôi</h4>
            <p>Nếu bạn có bất kỳ câu hỏi hoặc phản hồi nào, hãy liên hệ với chúng tôi:</p>
            <p>Email: covo488@gmail.com hoặc daoduycuong2k3@gmail.com</p>
            <p>Phone: 0363631682</p>
        </div>
    </div>

    <script>
        const firebaseConfig = {
            apiKey: "AIzaSyAy3lTCpTJ-t0fs4CA36WazSDcKN6VP4xg",
            authDomain: "iot-2024-b888a.firebaseapp.com",
            databaseURL: "https://iot-2024-b888a-default-rtdb.firebaseio.com",
            projectId: "iot-2024-b888a",
            storageBucket: "iot-2024-b888a.appspot.com",
            messagingSenderId: "954868204016",
            appId: "1:954868204016:web:4da827c214c12fead09d35",
            measurementId: "G-2H4YDJKYHF"
        };

        firebase.initializeApp(firebaseConfig);
        const database = firebase.database();
        const PASSWORD = "123456";

        let isGateInOpen = false;
        let isGateOutOpen = false;  // Cần để riêng biệt cho cổng vào và ra

        function toggleGate(gate, isOpen) {
            const path = gate === 'in' ? 'iotdata1/in/button' : 'iotdata1/out/button';
            database.ref(path).set(isOpen);
        }

        document.getElementById('open-gate-in').addEventListener('click', () => {
            const enteredPassword = prompt("Nhập mật khẩu để mở cửa vào:");
            if (enteredPassword === PASSWORD) {
                isGateInOpen = !isGateInOpen;
                toggleGate('in', isGateInOpen);
                document.getElementById('open-gate-in').textContent = isGateInOpen ? 'Đã Mở Cửa Vào' : 'Mở Cửa Vào';
            } else {
                alert("Mật khẩu không đúng!");
            }
        });

        document.getElementById('open-gate-out').addEventListener('click', () => {
            const enteredPassword = prompt("Nhập mật khẩu để mở cửa ra:");
            if (enteredPassword === PASSWORD) {
                isGateInOpen = !isGateInOpen;  // Chỉnh sửa từ isGateInOpen thành isGateOutOpen
                toggleGate('out', isGateInOpen);  // Cập nhật đến 'out' thay vì 'in'
                document.getElementById('open-gate-out').textContent = isGateInOpen ? 'Đã Mở Cửa Ra' : 'Mở Cửa Ra';
            } else {
                alert("Mật khẩu không đúng!");
            }
        });

        const dataRef = database.ref('iotdata1');
        dataRef.on('value', (snapshot) => {
            const data = snapshot.val();
            document.getElementById('in-license-plate').textContent = data.in?.licensePlate || "Không có dữ liệu";
            document.getElementById('in-date').textContent = data.in?.date || "Không có dữ liệu";
            document.getElementById('in-time').textContent = data.in?.time || "Không có dữ liệu";

            document.getElementById('out-license-plate').textContent = data.in?.licensePlate || "Không có dữ liệu";
            document.getElementById('out-date').textContent = data.in?.date || "Không có dữ liệu";
            document.getElementById('out-time').textContent = data.in?.time || "Không có dữ liệu";

            if (data.history) {
                const carList = document.getElementById('car-list');
                carList.innerHTML = "";

                let currentCarCount = 0;
                Object.keys(data.history).forEach((key, index) => {
                    const record = data.history[key];
                    if (!record.outTime) {
                        currentCarCount++;
                    }

                    const row = `
                        <tr>
                            <td>${index + 1}</td>
                            <td>${record.licensePlate1 || "Không có dữ liệu"}</td>
                            <td>${record.inTime || "Không có dữ liệu"}</td>
                            <td>${record.outTime || "Không có dữ liệu"}</td>
                        </tr>
                    `;
                    carList.insertAdjacentHTML('beforeend', row);
                });

                const totalSlots = 100;
                document.getElementById('current-car-count').textContent = currentCarCount;
                document.getElementById('available-spots').textContent = totalSlots - currentCarCount;
            }
        });
        document.getElementById('switch-to-web2').addEventListener('click', () => {
    window.location.href = '2.html'; // Replace with your Web 2 URL
});
    </script>
</body>
</html>
