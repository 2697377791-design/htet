<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>C50-Module shop 3D打印签收管理系统</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft YaHei", sans-serif;
        }

        body {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 40%, #0f3460 100%);
            color: #333;
            padding-top: 100px;
            min-height: 100vh;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }

        /* 固定头部 */
        .fixed-header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            z-index: 1000;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .header-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
            color: #2d8cf0;
        }

        /* 选项卡 */
        .tabs {
            display: flex;
            margin-bottom: 20px;
            border-bottom: 2px solid #e0e0e0;
        }

        .tab {
            padding: 12px 24px;
            cursor: pointer;
            font-size: 16px;
            font-weight: 500;
            color: #666;
            border-bottom: 3px solid transparent;
            transition: all 0.3s;
        }

        .tab.active {
            color: #2d8cf0;
            border-bottom-color: #2d8cf0;
        }

        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
        }

        /* 功能卡片 */
        .card {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 12px;
            padding: 25px;
            margin-bottom: 25px;
            box-shadow: 0 2px 12px rgba(0,0,0,0.08);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .card-title {
            font-size: 18px;
            margin-bottom: 20px;
            color: #444;
            border-left: 4px solid #2d8cf0;
            padding-left: 10px;
        }

        /* 表单样式 */
        .form-group {
            margin-bottom: 18px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        input, select {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-size: 16px;
            outline: none;
            transition: border 0.3s;
        }

        input:focus, select:focus {
            border-color: #2d8cf0;
        }

        /* 按钮 */
        .btn {
            padding: 12px 25px;
            border: none;
            border-radius: 6px;
            font-size: 16px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn-primary {
            background-color: #2d8cf0;
            color: white;
        }

        .btn-primary:hover {
            background-color: #1b79d8;
        }

        .btn-success {
            background-color: #00c48c;
            color: white;
        }

        .btn-success:hover {
            background-color: #00b37e;
        }

        .btn-warning {
            background-color: #ff9500;
            color: white;
        }

        .btn-warning:hover {
            background-color: #e68a00;
        }

        /* 运单信息 */
        .order-info {
            padding: 15px;
            background: #f8f9fa;
            border-radius: 8px;
            margin: 15px 0;
            line-height: 1.7;
        }

        .status {
            padding: 4px 10px;
            border-radius: 4px;
            font-size: 14px;
        }

        .status-wait {
            background: #fff5cc;
            color: #d48806;
        }

        .status-transport {
            background: #e6f7ff;
            color: #1890ff;
        }

        .status-sign {
            background: #e6fffb;
            color: #00b494;
        }

        /* 物流进度条 */
        .progress-container {
            margin: 20px 0;
            padding: 10px 0;
        }

        .progress-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
            margin-bottom: 15px;
        }

        .progress-bar::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 0;
            transform: translateY(-50%);
            height: 4px;
            width: 100%;
            background-color: #e0e0e0;
            z-index: 1;
        }

        .progress-line {
            position: absolute;
            top: 50%;
            left: 0;
            transform: translateY(-50%);
            height: 4px;
            background-color: #2d8cf0;
            transition: width 0.5s ease;
            z-index: 2;
        }

        .progress-step {
            width: 30px;
            height: 30px;
            background-color: #fff;
            border: 3px solid #e0e0e0;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: #999;
            position: relative;
            z-index: 3;
            transition: all 0.3s;
        }

        .progress-step.active {
            border-color: #2d8cf0;
            background-color: #2d8cf0;
            color: white;
        }

        .progress-labels {
            display: flex;
            justify-content: space-between;
            padding: 0 5px;
        }

        .progress-label {
            width: 25%;
            text-align: center;
            font-size: 13px;
            color: #999;
        }

        .progress-label.active {
            color: #2d8cf0;
            font-weight: 500;
        }

        /* 签收记录表格 */
        .table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }

        .table th, .table td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #eee;
        }

        .table th {
            background-color: #f8f9fa;
            font-weight: 500;
        }

        /* 空数据提示 */
        .empty {
            text-align: center;
            padding: 30px 0;
            color: #999;
        }
    </style>
</head>
<body>
    <div class="fixed-header">
        <div class="header-content">
            <h1>C50-Module shop 3D打印签收管理系统</h1>
            <p>快速查询 · 一键签收 · 新建运单 · 进度可控</p>
        </div>
    </div>

    <div class="container">
        <div style="margin-bottom: 20px; text-align: right;">
            <button class="btn btn-warning" onclick="checkPassword()">新建运单</button>
        </div>
            <!-- 运单查询模块 -->
            <div class="card">
                <div class="card-title">运单查询 & 物流进度</div>
                <div class="form-group">
                    <label>运单号</label>
                    <input type="text" id="orderNo" placeholder="请输入运单号" value="WL2025001">
                </div>
                <button class="btn btn-primary" onclick="searchOrder()">查询运单</button>

                <div id="orderInfo" class="order-info" style="display: none;">
                    <p><strong>运单号：</strong><span id="showOrderNo"></span></p>
                    <p><strong>项目名称：</strong><span id="showName"></span></p>
                    <p><strong>打印创建时间：</strong><span id="showPhone"></span></p>
                    <p><strong>预计打印时间：</strong><span id="showAddress"></span></p>
                    <p><strong>当前状态：</strong><span id="showStatus" class="status"></span></p>

                    <!-- 物流进度条 -->
                    <div class="progress-container">
                        <div class="progress-bar">
                        <div class="progress-line" id="progressLine"></div>
                        <div class="progress-step" id="step1">1</div>
                        <div class="progress-step" id="step2">2</div>
                        <div class="progress-step" id="step3">3</div>
                    </div>
                        <div class="progress-labels">
                        <div class="progress-label" id="label1">打印中</div>
                        <div class="progress-label" id="label2">派送中</div>
                        <div class="progress-label" id="label3">已签收</div>
                    </div>
                    </div>


                </div>
            </div>

            <!-- 签收模块 -->
            <div class="card">
                <div class="card-title">货物签收</div>
                <div class="form-group">
                    <label>签收人姓名</label>
                    <input type="text" id="signName" placeholder="请输入签收人姓名">
                </div>
                <div class="form-group">
                    <label>签收图片</label>
                    <input type="file" id="signImage" accept="image/*">
                </div>
                <button class="btn btn-success" onclick="signOrder()">确认签收</button>
            </div>

            <!-- 签收记录 -->
            <div class="card">
                <div class="card-title">签收记录</div>
                <table class="table" id="recordTable">
                    <thead>
                        <tr>
                            <th>运单号</th>
                            <th>项目名称</th>
                            <th>签收人</th>
                            <th>签收时间</th>
                            <th>状态</th>
                            <th>操作</th>
                            <th>签收图片</th>
                        </tr>
                    </thead>
                    <tbody id="recordBody">
                        <tr><td colspan="6" class="empty">暂无签收记录</td></tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>

    <script>
        // 运单数据
        let orderData = [];

        // 签收记录
        let signRecords = [];

        // 加载运单数据
        function loadOrderData() {
            const savedData = localStorage.getItem('orderData');
            if (savedData) {
                orderData = JSON.parse(savedData);
            } else {
                // 初始化默认数据
                orderData = [
                    {
                        orderNo: "WL2025001",
                        name: "张三",
                        phone: "13800138000",
                        address: "北京市朝阳区XX小区1号楼",
                        status: "打印中",
                        progress: 1
                    },
                    {
                        orderNo: "WL2025002",
                        name: "李四",
                        phone: "13900139000",
                        address: "上海市浦东新区XX路",
                        status: "派送中",
                        progress: 2
                    }
                ];
                saveOrderData();
            }
        }

        // 保存运单数据
        function saveOrderData() {
            localStorage.setItem('orderData', JSON.stringify(orderData));
        }

        // 加载签收记录
        function loadSignRecords() {
            const savedRecords = localStorage.getItem('signRecords');
            if (savedRecords) {
                signRecords = JSON.parse(savedRecords);
                renderRecords();
            }
        }

        // 保存签收记录
        function saveSignRecords() {
            localStorage.setItem('signRecords', JSON.stringify(signRecords));
        }

        // 密码验证
        function checkPassword() {
            const password = prompt('请输入管理员密码：');
            if (password === '44944') {
                localStorage.setItem('orderCreateAuth', 'true');
                window.location.href = 'create_order.html';
            } else {
                alert('密码错误，无法访问新建运单页面！');
            }
        }

        // 查询运单
        function searchOrder() {
            const orderNo = document.getElementById("orderNo").value.trim();
            if (!orderNo) {
                alert("请输入运单号！");
                return;
            }

            const order = orderData.find(item => item.orderNo === orderNo);
            if (!order) {
                alert("未找到该运单！");
                document.getElementById("orderInfo").style.display = "none";
                return;
            }

            document.getElementById("showOrderNo").innerText = order.orderNo;
            document.getElementById("showName").innerText = order.name;
            document.getElementById("showPhone").innerText = order.phone;
            document.getElementById("showAddress").innerText = order.address;
            
            const statusEl = document.getElementById("showStatus");
            statusEl.innerText = order.status;
            
            if(order.status === "打印中") {
                statusEl.className = "status status-wait";
            } else if(order.status === "派送中") {
                statusEl.className = "status status-transport";
            } else {
                statusEl.className = "status status-sign";
            }

            renderProgress(order.progress);
            document.getElementById("orderInfo").style.display = "block";
        }

        // 渲染进度条
        function renderProgress(step) {
            const line = document.getElementById("progressLine");
            const percent = (step - 1) * 50;
            line.style.width = percent + "%";

            document.querySelectorAll('.progress-step').forEach((el, index) => {
                el.classList.remove('active');
                document.querySelectorAll('.progress-label')[index].classList.remove('active');
            });

            for(let i=0; i<step; i++) {
                document.getElementById(`step${i+1}`).classList.add('active');
                document.getElementById(`label${i+1}`).classList.add('active');
            }
        }

        // 确认签收
        function signOrder() {
            const orderNo = document.getElementById("orderNo").value.trim();
            const signName = document.getElementById("signName").value.trim();
            const signImage = document.getElementById("signImage").files[0];

            if (!orderNo || !signName) {
                alert("请先查询运单并填写签收人！");
                return;
            }

            const order = orderData.find(item => item.orderNo === orderNo);
            if (!order) {
                alert("运单不存在！");
                return;
            }

            if (order.status === "已签收") {
                alert("该运单已签收！");
                return;
            }

            order.status = "已签收";
            order.progress = 3;

            // 处理图片上传
            let imageData = null;
            if (signImage) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    imageData = e.target.result;
                    completeSignOrder(order, signName, imageData);
                };
                reader.readAsDataURL(signImage);
            } else {
                completeSignOrder(order, signName, null);
            }
        }

        // 完成签收操作
        function completeSignOrder(order, signName, imageData) {
            const record = {
                orderNo: order.orderNo,
                name: order.name,
                signName: signName,
                time: new Date().toLocaleString(),
                status: "已签收",
                image: imageData
            };
            signRecords.unshift(record);

            saveOrderData();
            saveSignRecords();

            searchOrder();
            renderRecords();
            document.getElementById("signName").value = "";
            document.getElementById("signImage").value = "";
            alert("签收成功！");
        }



        // 渲染记录
        function renderRecords() {
            const body = document.getElementById("recordBody");
            if (signRecords.length === 0) {
                body.innerHTML = `<tr><td colspan="7" class="empty">暂无签收记录</td></tr>`;
                return;
            }

            let html = "";
            signRecords.forEach((item, index) => {
                let imageHtml = "无图片";
                if (item.image) {
                    imageHtml = `<img src="${item.image}" style="width: 80px; height: 60px; object-fit: cover; border-radius: 4px;">`;
                }
                html += `
                    <tr>
                        <td>${item.orderNo}</td>
                        <td>${item.name}</td>
                        <td>${item.signName}</td>
                        <td>${item.time}</td>
                        <td><span class="status status-sign">${item.status}</span></td>
                        <td><button class="btn btn-warning" onclick="deleteRecord(${index})">删除</button></td>
                        <td>${imageHtml}</td>
                    </tr>
                `;
            });
            body.innerHTML = html;
        }

        // 删除签收记录
        function deleteRecord(index) {
            if (confirm("确定要删除这条签收记录吗？")) {
                signRecords.splice(index, 1);
                saveSignRecords();
                renderRecords();
                alert("记录删除成功！");
            }
        }

        window.onload = function() {
            loadOrderData();
            loadSignRecords();
            searchOrder();
        };
    </script>
    <footer style="text-align: center; margin-top: 40px; padding: 20px; background-color: #f8f9fa; border-top: 1px solid #e9ecef;">
        <p>作者:Htet 出品</p>
    </footer>
</body>
</html>
