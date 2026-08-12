<!DOCTYPE html>
<html lang="ps" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>د صرافۍ او حوالو مدیریت سسټم</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
        }
        body {
            background-color: #f4f6f9;
            color: #333;
            padding: 15px;
        }
        .header {
            background-color: #1e293b;
            color: #fff;
            text-align: center;
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .card {
            background: #ffffff;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .card h2 {
            font-size: 1.1rem;
            color: #0f172a;
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 8px;
            margin-bottom: 15px;
        }
        .form-group {
            margin-bottom: 12px;
        }
        label {
            display: block;
            font-size: 0.9rem;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 10px;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            font-size: 0.95rem;
        }
        button {
            width: 100%;
            background-color: #2563eb;
            color: white;
            border: none;
            padding: 12px;
            border-radius: 6px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
        }
        button:active {
            background-color: #1d4ed8;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
            font-size: 0.85rem;
        }
        th, td {
            border: 1px solid #cbd5e1;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f1f5f9;
        }
        .status-pending {
            color: #d97706;
            font-weight: bold;
        }
        .status-paid {
            color: #16a34a;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <div class="header">
        <h1>د صرافۍ او حوالو سسټم</h1>
    </div>

    <!-- Currency Converter / د اسعارو بدلول -->
    <div class="card">
        <h2>د اسعارو محاسبه (Exchange Calculator)</h2>
        <div class="form-group">
            <label>مبلغ (مقدار):</label>
            <input type="number" id="calcAmount" placeholder="مثلاً: 100">
        </div>
        <div class="form-group">
            <label>نرخ (Exchange Rate):</label>
            <input type="number" id="calcRate" placeholder="مثلاً: 70.5">
        </div>
        <button onclick="calculateCurrency()">حساب کړئ</button>
        <h3 id="calcResult" style="margin-top:10px; color:#2563eb; text-align:center;"></h3>
    </div>

    <!-- Hawala Registration / د حوالې ثبتول -->
    <div class="card">
        <h2>د نوې حوالې ثبتول (New Hawala)</h2>
        <form id="hawalaForm">
            <div class="form-group">
                <label>د لیږونکي نوم (Sender):</label>
                <input type="text" id="sender" required placeholder="احمد">
            </div>
            <div class="form-group">
                <label>د ترلاسه کونکي نوم (Receiver):</label>
                <input type="text" id="receiver" required placeholder="محمود">
            </div>
            <div class="form-group">
                <label>مبلغ (Amount):</label>
                <input type="number" id="amount" required placeholder="500">
            </div>
            <div class="form-group">
                <label>اسعار (Currency):</label>
                <select id="currency">
                    <option value="USD">ډالر ($)</option>
                    <option value="AFN">افغانۍ (؋)</option>
                    <option value="PKR">کلدارې (Rs)</option>
                </select>
            </div>
            <div class="form-group">
                <label>منزل / ولایت (Destination):</label>
                <input type="text" id="destination" required placeholder="کابل / کندهار">
            </div>
            <button type="button" onclick="addHawala()">حواله ثبت کړئ</button>
        </form>
    </div>

    <!-- Ledger Table / د حوالو لیست -->
    <div class="card">
        <h2>د ثبت شویو حوالو لیست</h2>
        <div style="overflow-x:auto;">
            <table>
                <thead>
                    <tr>
                        <th>کوډ</th>
                        <th>لیږونکی</th>
                        <th>ترلاسه کونکی</th>
                        <th>مبلغ</th>
                        <th>ولایت</th>
                        <th>حالت</th>
                    </tr>
                </thead>
                <tbody id="hawalaTable">
                    <!-- Transactions will load here dynamically -->
                </tbody>
            </table>
        </div>
    </div>

    <script>
        // Currency Calculator Function
        function calculateCurrency() {
            let amount = document.getElementById('calcAmount').value;
            let rate = document.getElementById('calcRate').value;
            if(amount && rate) {
                let total = amount * rate;
                document.getElementById('calcResult').innerText = "مجموعه: " + total.toFixed(2);
            } else {
                document.getElementById('calcResult').innerText = "مهرباني وکړئ دواړه خانې ډکې کړئ.";
            }
        }

        // Add Hawala Function
        let hawalaList = [];

        function addHawala() {
            let sender = document.getElementById('sender').value;
            let receiver = document.getElementById('receiver').value;
            let amount = document.getElementById('amount').value;
            let currency = document.getElementById('currency').value;
            let destination = document.getElementById('destination').value;

            if(!sender || !receiver || !amount || !destination) {
                alert("مهرباني وکړئ ټول معلومات ورسوئ.");
                return;
            }

            // Generate random 5-digit Hawala code
            let code = "HW-" + Math.floor(10000 + Math.random() * 90000);

            let transaction = {
                code: code,
                sender: sender,
                receiver: receiver,
                amount: amount + " " + currency,
                destination: destination,
                status: "پاتې (Pending)"
            };

            hawalaList.push(transaction);
            renderTable();

            // Clear inputs
            document.getElementById('hawalaForm').reset();
        }

        function renderTable() {
            let tbody = document.getElementById('hawalaTable');
            tbody.innerHTML = "";

            hawalaList.forEach((item, index) => {
                let row = `<tr>
                    <td><b>${item.code}</b></td>
                    <td>${item.sender}</td>
                    <td>${item.receiver}</td>
                    <td>${item.amount}</td>
                    <td>${item.destination}</td>
                    <td class="status-pending">${item.status}</td>
                </tr>`;
                tbody.innerHTML += row;
            });
        }
    </script>
</body>
</html>
