<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hanami Cafe - Japanese Inspired Coffee & Tea</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" />
    <style>
        /* Reset dan Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #8B4513;
            --secondary: #D4AF37;
            --accent: #C41E3A;
            --light: #F5F5DC;
            --dark: #3C2F2F;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--primary);
            color: white;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            color: var(--secondary);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 25px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            padding: 5px 10px;
            border-radius: 4px;
        }

        nav ul li a:hover {
            color: var(--secondary);
        }

        nav ul li a.active {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--secondary);
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 22px;
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: var(--accent);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: bold;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1554118811-1e0d58224f24?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1447&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            margin-bottom: 50px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto 30px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
        }

        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: var(--dark);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }

        .btn:hover {
            background-color: #e6c12e;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .btn:disabled {
            background-color: #ccc;
            cursor: not-allowed;
            transform: none;
        }

        /* Section Styles */
        section {
            padding: 60px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        .section-title h2 {
            font-size: 36px;
            color: var(--primary);
            display: inline-block;
            padding-bottom: 10px;
        }

        .section-title h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 3px;
            background-color: var(--secondary);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }

        /* Menu Section */
        .menu-categories {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .category-btn {
            background: none;
            border: 2px solid var(--primary);
            color: var(--primary);
            padding: 8px 20px;
            margin: 5px 10px;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
        }

        .category-btn.active, .category-btn:hover {
            background-color: var(--primary);
            color: white;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }

        .menu-item {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
            cursor: pointer;
        }

        .menu-item:hover {
            transform: translateY(-5px);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .menu-item-content {
            padding: 20px;
        }

        .menu-item h3 {
            font-size: 20px;
            margin-bottom: 10px;
            color: var(--primary);
        }

        .menu-item p {
            color: #666;
            margin-bottom: 15px;
            font-size: 14px;
        }

        .menu-item-price {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .price {
            font-weight: bold;
            color: var(--primary);
            font-size: 18px;
        }

        .add-to-cart {
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .add-to-cart:hover {
            background-color: var(--accent);
        }

        /* Modal Item Detail */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background-color: white;
            border-radius: 10px;
            max-width: 500px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
        }

        .modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: var(--dark);
            z-index: 1;
        }

        .modal-header {
            position: relative;
        }

        .modal-header img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 10px 10px 0 0;
        }

        .modal-body {
            padding: 20px;
        }

        .modal-title {
            font-size: 24px;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .modal-price {
            font-size: 20px;
            font-weight: bold;
            color: var(--primary);
            margin-bottom: 15px;
        }

        .modal-description {
            margin-bottom: 20px;
            color: #666;
        }

        .customization-options {
            margin-bottom: 20px;
        }

        .option-group {
            margin-bottom: 15px;
        }

        .option-title {
            font-weight: bold;
            margin-bottom: 8px;
            color: var(--dark);
        }

        .option-items {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .option-item {
            border: 1px solid #ddd;
            padding: 8px 15px;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 14px;
        }

        .option-item.selected {
            background-color: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .special-request {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-top: 10px;
            resize: vertical;
        }

        .char-count {
            font-size: 12px;
            color: #666;
            text-align: right;
            margin-top: 5px;
        }

        .modal-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .quantity-selector {
            display: flex;
            align-items: center;
        }

        .qty-btn {
            width: 35px;
            height: 35px;
            border: 1px solid #ddd;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 18px;
        }

        .qty-minus {
            border-radius: 5px 0 0 5px;
        }

        .qty-plus {
            border-radius: 0 5px 5px 0;
        }

        .qty-value {
            width: 50px;
            height: 35px;
            border-top: 1px solid #ddd;
            border-bottom: 1px solid #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* Cart Sidebar */
        .cart-sidebar {
            position: fixed;
            top: 0;
            right: -400px;
            width: 380px;
            height: 100vh;
            background-color: white;
            box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);
            transition: right 0.3s ease-in-out;
            z-index: 1000;
            display: flex;
            flex-direction: column;
        }

        .cart-sidebar.active {
            right: 0;
        }

        .cart-header {
            padding: 20px;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .cart-header h3 {
            color: var(--primary);
        }

        .close-cart {
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: #666;
        }

        .cart-items {
            flex: 1;
            overflow-y: auto;
            padding: 20px;
        }

        .cart-item {
            display: flex;
            margin-bottom: 15px;
            padding-bottom: 15px;
            border-bottom: 1px solid #eee;
        }

        .cart-item img {
            width: 80px;
            height: 80px;
            object-fit: cover;
            border-radius: 5px;
            margin-right: 15px;
        }

        .cart-item-details {
            flex: 1;
        }

        .cart-item-details h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }

        .cart-item-price {
            color: var(--dark);
            font-weight: bold;
            margin-bottom: 10px;
        }

        .cart-item-customization {
            font-size: 12px;
            color: #666;
            margin-bottom: 5px;
        }

        .cart-item-quantity {
            display: flex;
            align-items: center;
        }

        .quantity-btn {
            background-color: #f0f0f0;
            border: none;
            width: 25px;
            height: 25px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
        }

        .quantity {
            margin: 0 10px;
            font-weight: bold;
        }

        .remove-item {
            color: var(--accent);
            background: none;
            border: none;
            cursor: pointer;
            margin-left: 10px;
        }

        .cart-footer {
            padding: 20px;
            border-top: 1px solid #eee;
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            font-size: 18px;
            font-weight: bold;
        }

        .checkout-btn {
            width: 100%;
            padding: 12px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .checkout-btn:hover {
            background-color: var(--accent);
        }

        /* Payment Page */
        .payment-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .payment-steps {
            display: flex;
            justify-content: space-between;
            margin-bottom: 30px;
            position: relative;
        }

        .payment-steps:before {
            content: '';
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 2px;
            background-color: #eee;
            z-index: 1;
        }

        .step {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .step-number {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #eee;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 10px;
            font-weight: bold;
            color: #666;
        }

        .step.active .step-number {
            background-color: var(--primary);
            color: white;
        }

        .step.completed .step-number {
            background-color: var(--secondary);
            color: white;
        }

        .step-label {
            font-size: 14px;
            color: #666;
        }

        .step.active .step-label {
            color: var(--primary);
            font-weight: bold;
        }

        .payment-form {
            margin-bottom: 30px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .form-group input.error, .form-group textarea.error {
            border-color: var(--accent);
        }

        .error-message {
            color: var(--accent);
            font-size: 14px;
            margin-top: 5px;
        }

        .delivery-options {
            margin-bottom: 20px;
        }

        .delivery-option {
            border: 2px solid #eee;
            border-radius: 5px;
            padding: 15px;
            margin-bottom: 10px;
            cursor: pointer;
            transition: all 0.3s;
        }

        .delivery-option.selected {
            border-color: var(--primary);
            background-color: rgba(139, 69, 19, 0.05);
        }

        .delivery-option-header {
            display: flex;
            justify-content: between;
            align-items: center;
            margin-bottom: 10px;
        }

        .delivery-option-name {
            font-weight: bold;
            color: var(--primary);
        }

        .delivery-option-price {
            font-weight: bold;
        }

        .delivery-option-desc {
            font-size: 14px;
            color: #666;
        }

        .payment-methods {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-bottom: 30px;
        }

        .payment-method {
            border: 2px solid #eee;
            border-radius: 5px;
            padding: 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
        }

        .payment-method:hover, .payment-method.selected {
            border-color: var(--primary);
            background-color: rgba(139, 69, 19, 0.05);
        }

        .payment-method i {
            font-size: 30px;
            margin-bottom: 10px;
            color: var(--primary);
        }

        .payment-instructions {
            background-color: #f0f8ff;
            padding: 15px;
            border-radius: 5px;
            margin-top: 10px;
            display: none;
        }

        .payment-instructions.active {
            display: block;
        }

        .payment-instructions p {
            margin-bottom: 10px;
            font-size: 14px;
        }

        .qris-code {
            text-align: center;
            margin: 15px 0;
        }

        .qris-code img {
            max-width: 200px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .virtual-account {
            background-color: #e6f7ff;
            padding: 10px;
            border-radius: 5px;
            font-family: monospace;
            font-size: 16px;
            text-align: center;
            margin-bottom: 10px;
        }

        .order-summary {
            background-color: #f9f9f9;
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 30px;
        }

        .order-summary h3 {
            margin-bottom: 15px;
            color: var(--primary);
        }

        .summary-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }

        .summary-total {
            border-top: 1px solid #ddd;
            padding-top: 10px;
            margin-top: 10px;
            font-weight: bold;
            font-size: 18px;
        }

        .payment-actions {
            display: flex;
            justify-content: space-between;
        }

        .back-btn {
            background-color: #eee;
            color: #333;
        }

        .back-btn:hover {
            background-color: #ddd;
        }

        /* Tracking Page */
        .tracking-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .tracking-steps {
            display: flex;
            justify-content: space-between;
            margin: 40px 0;
            position: relative;
        }

        .tracking-steps:before {
            content: '';
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 3px;
            background-color: #eee;
            z-index: 1;
        }

        .tracking-step {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            z-index: 2;
            text-align: center;
        }

        .tracking-step-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #eee;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .tracking-step.active .tracking-step-icon {
            background-color: var(--primary);
            color: white;
        }

        .tracking-step.completed .tracking-step-icon {
            background-color: var(--secondary);
            color: white;
        }

        .tracking-step-label {
            font-size: 14px;
            font-weight: bold;
        }

        .tracking-info {
            background-color: #f9f9f9;
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 30px;
        }

        .tracking-map {
            height: 300px;
            background-color: #eee;
            border-radius: 5px;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .driver-info {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .driver-photo {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: #ddd;
            margin-right: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }

        .driver-details h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }

        .estimated-time {
            font-size: 18px;
            font-weight: bold;
            text-align: center;
            margin: 20px 0;
            color: var(--primary);
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-column h3 {
            font-size: 20px;
            margin-bottom: 20px;
            color: var(--secondary);
        }

        .footer-column p, .footer-column a {
            color: #ccc;
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-column a:hover {
            color: var(--secondary);
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-icons a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: background-color 0.3s;
        }

        .social-icons a:hover {
            background-color: var(--secondary);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #aaa;
            font-size: 14px;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
            
            .cart-sidebar {
                width: 100%;
                right: -100%;
            }
            
            .payment-methods {
                grid-template-columns: 1fr;
            }
            
            .modal-content {
                width: 95%;
            }
            
            .tracking-steps {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .tracking-steps:before {
                display: none;
            }
            
            .tracking-step {
                flex-direction: row;
                margin-bottom: 20px;
                width: 100%;
            }
            
            .tracking-step-icon {
                margin-right: 15px;
                margin-bottom: 0;
            }
        }

        /* Page Navigation */
        .page {
            display: none;
        }
        
        .page.active {
            display: block;
        }
        
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 999;
            display: none;
        }
        
        .overlay.active {
            display: block;
        }

        /* Map Container */
        #map {
            height: 300px;
            width: 100%;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <!-- Overlay untuk sidebar -->
    <div class="overlay" id="overlay"></div>

    <!-- Modal untuk detail item -->
    <div class="modal" id="item-modal">
        <div class="modal-content">
            <button class="modal-close" id="modal-close">&times;</button>
            <div class="modal-header">
                <img id="modal-image" src="" alt="">
            </div>
            <div class="modal-body">
                <h2 class="modal-title" id="modal-title"></h2>
                <div class="modal-price" id="modal-price"></div>
                <p class="modal-description" id="modal-description"></p>
                
                <div class="customization-options">
                    <div class="option-group">
                        <div class="option-title">Takaran Gula</div>
                        <div class="option-items">
                            <div class="option-item" data-value="normal">Normal</div>
                            <div class="option-item" data-value="less">Kurang Manis</div>
                            <div class="option-item" data-value="none">Tanpa Gula</div>
                            <div class="option-item" data-value="extra">Extra Manis</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Takaran Es</div>
                        <div class="option-items">
                            <div class="option-item" data-value="normal">Normal</div>
                            <div class="option-item" data-value="less">Kurang Es</div>
                            <div class="option-item" data-value="none">Tanpa Es</div>
                            <div class="option-item" data-value="extra">Extra Es</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Additional Topping</div>
                        <div class="option-items">
                            <div class="option-item" data-value="boba">Boba (+Rp 5,000)</div>
                            <div class="option-item" data-value="grassjelly">Grass Jelly (+Rp 4,000)</div>
                            <div class="option-item" data-value="pudding">Pudding (+Rp 6,000)</div>
                            <div class="option-item" data-value="cheese">Cheese Foam (+Rp 8,000)</div>
                            <div class="option-item" data-value="onsen">Onsen Tamago (+Rp 7,000)</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Perlengkapan Wajib*</div>
                        <div class="option-items">
                            <div class="option-item selected" data-value="utensils">Sendok & Garpu/Sumpit (+Rp 1,500)</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Request Khusus</div>
                        <textarea class="special-request" id="special-request" placeholder="Contoh: Susu almond, ekstra hot, dll." maxlength="80"></textarea>
                        <div class="char-count"><span id="char-count">0</span>/80 karakter</div>
                    </div>
                </div>
                
                <div class="modal-actions">
                    <div class="quantity-selector">
                        <button class="qty-btn qty-minus">-</button>
                        <div class="qty-value">1</div>
                        <button class="qty-btn qty-plus">+</button>
                    </div>
                    <button class="btn" id="add-to-cart-modal">Tambah ke Keranjang</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <i class="fas fa-leaf"></i>
                <span>Hanami Cafe</span>
            </div>
            <nav>
                <ul>
                    <li><a href="#" class="nav-link active" data-page="home">Beranda</a></li>
                    <li><a href="#" class="nav-link" data-page="menu">Menu</a></li>
                    <li><a href="#" class="nav-link" data-page="about">Tentang Kami</a></li>
                    <li><a href="#" class="nav-link" data-page="contact">Kontak</a></li>
                </ul>
            </nav>
            <div class="cart-icon" id="cart-icon">
                <i class="fas fa-shopping-cart"></i>
                <span class="cart-count">0</span>
            </div>
        </div>
    </header>

    <!-- Home Page -->
    <section class="page active" id="home">
        <div class="hero">
            <h1>Selamat Datang di Hanami Cafe</h1>
            <p>Nikmati pengalaman kopi dan teh Jepang yang autentik dengan sentuhan modern di tengah suasana yang menenangkan.</p>
            <a href="#" class="btn nav-link" data-page="menu">Lihat Menu</a>
        </div>

        <div class="container">
            <div class="section-title">
                <h2>Menu Spesial Kami</h2>
            </div>
            <div class="menu-grid">
                <!-- Item menu akan ditampilkan di sini -->
            </div>
        </div>
    </section>

    <!-- Menu Page -->
    <section class="page" id="menu">
        <div class="container">
            <div class="section-title">
                <h2>Menu Lengkap</h2>
            </div>
            
            <div class="menu-categories">
                <button class="category-btn active" data-category="all">Semua</button>
                <button class="category-btn" data-category="coffee">Kopi</button>
                <button class="category-btn" data-category="tea">Teh</button>
                <button class="category-btn" data-category="dessert">Dessert</button>
                <button class="category-btn" data-category="food">Makanan</button>
            </div>
            
            <div class="menu-grid" id="menu-container">
                <!-- Item menu akan ditampilkan di sini -->
            </div>
        </div>
    </section>

    <!-- Payment Page -->
    <section class="page" id="payment">
        <div class="container">
            <div class="section-title">
                <h2>Checkout</h2>
            </div>
            
            <div class="payment-container">
                <div class="payment-steps">
                    <div class="step completed">
                        <div class="step-number">1</div>
                        <div class="step-label">Keranjang</div>
                    </div>
                    <div class="step active">
                        <div class="step-number">2</div>
                        <div class="step-label">Pembayaran</div>
                    </div>
                    <div class="step">
                        <div class="step-number">3</div>
                        <div class="step-label">Selesai</div>
                    </div>
                </div>
                
                <div class="payment-form">
                    <h3>Informasi Pengiriman</h3>
                    <div class="form-group">
                        <label for="name">Nama Lengkap *</label>
                        <input type="text" id="name" placeholder="Masukkan nama lengkap (maks. 20 huruf)" maxlength="20">
                        <div class="error-message" id="name-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="phone">Nomor Telepon *</label>
                        <input type="tel" id="phone" placeholder="Contoh: 081234567890">
                        <div class="error-message" id="phone-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="email">Email *</label>
                        <input type="email" id="email" placeholder="email@contoh.com">
                        <div class="error-message" id="email-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="address">Alamat Pengiriman *</label>
                        <textarea id="address" rows="3" placeholder="Masukkan alamat lengkap"></textarea>
                        <div class="error-message" id="address-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="notes">Catatan (opsional, maks. 80 huruf)</label>
                        <textarea id="notes" rows="2" placeholder="Catatan khusus untuk pesanan" maxlength="80"></textarea>
                        <div class="char-count"><span id="notes-char-count">0</span>/80 karakter</div>
                    </div>
                </div>
                
                <h3>Pilihan Pengiriman</h3>
                <div class="delivery-options">
                    <div class="delivery-option selected" data-delivery="grabexpress">
                        <div class="delivery-option-header">
                            <span class="delivery-option-name">GrabExpress</span>
                            <span class="delivery-option-price" id="delivery-price">Rp 15,000</span>
                        </div>
                        <div class="delivery-option-desc">Estimasi: 30-45 menit • Gratis ongkir untuk order di atas Rp 75,000</div>
                    </div>
                </div>
                
                <h3>Metode Pembayaran</h3>
                <div class="payment-methods">
                    <div class="payment-method selected" data-method="gopay">
                        <i class="fas fa-wallet"></i>
                        <div>Gopay</div>
                    </div>
                    <div class="payment-method" data-method="qris">
                        <i class="fas fa-qrcode"></i>
                        <div>QRIS</div>
                    </div>
                    <div class="payment-method" data-method="va">
                        <i class="fas fa-university"></i>
                        <div>Virtual Account</div>
                    </div>
                </div>
                
                <!-- Instruksi Pembayaran -->
                <div class="payment-instructions active" id="gopay-instructions">
                    <p><strong>Instruksi Pembayaran Gopay:</strong></p>
                    <p>1. Buka aplikasi Gopay di smartphone Anda</p>
                    <p>2. Pilih "Bayar" dan scan QR code berikut</p>
                    <div class="qris-code">
                        <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=HANAMICAFE-ORDER-2024" alt="QR Code Gopay">
                    </div>
                    <p>3. Atau gunakan nomor virtual berikut: <strong>8080801234567890</strong></p>
                    <p>4. Jumlah yang harus dibayar: <strong id="gopay-amount">Rp 0</strong></p>
                </div>
                
                <div class="payment-instructions" id="qris-instructions">
                    <p><strong>Instruksi Pembayaran QRIS:</strong></p>
                    <p>1. Buka aplikasi e-wallet atau mobile banking Anda</p>
                    <p>2. Pilih fitur "Scan QRIS"</p>
                    <p>3. Scan QR code berikut</p>
                    <div class="qris-code">
                        <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=HANAMICAFE-QRIS-ORDER-2024" alt="QR Code QRIS">
                    </div>
                    <p>4. Jumlah yang harus dibayar: <strong id="qris-amount">Rp 0</strong></p>
                </div>
                
                <div class="payment-instructions" id="va-instructions">
                    <p><strong>Instruksi Pembayaran Virtual Account:</strong></p>
                    <p>1. Buka aplikasi mobile banking Anda</p>
                    <p>2. Pilih "Transfer" → "Virtual Account"</p>
                    <p>3. Masukkan nomor virtual account berikut:</p>
                    <div class="virtual-account">8080801234567890</div>
                    <p>4. Jumlah yang harus dibayar: <strong id="va-amount">Rp 0</strong></p>
                    <p>5. Transaksi akan diproses otomatis</p>
                </div>
                
                <div class="order-summary">
                    <h3>Ringkasan Pesanan</h3>
                    <div id="payment-summary">
                        <!-- Item pesanan akan ditampilkan di sini -->
                    </div>
                    <div class="summary-item">
                        <span>Ongkos Kirim</span>
                        <span id="delivery-cost">Rp 15,000</span>
                    </div>
                    <div class="summary-item summary-total">
                        <span>Total</span>
                        <span id="payment-total">Rp 0</span>
                    </div>
                </div>
                
                <div class="payment-actions">
                    <button class="btn back-btn" id="back-to-cart">Kembali ke Keranjang</button>
                    <button class="btn" id="confirm-payment">Bayar Sekarang</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Tracking Page -->
    <section class="page" id="tracking">
        <div class="container">
            <div class="section-title">
                <h2>Lacak Pesanan Anda</h2>
            </div>
            
            <div class="tracking-container">
                <div class="tracking-steps">
                    <div class="tracking-step completed">
                        <div class="tracking-step-icon"><i class="fas fa-utensils"></i></div>
                        <div class="tracking-step-label">Pesanan Diproses</div>
                    </div>
                    <div class="tracking-step active">
                        <div class="tracking-step-icon"><i class="fas fa-motorcycle"></i></div>
                        <div class="tracking-step-label">Driver Menuju Cafe</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-coffee"></i></div>
                        <div class="tracking-step-label">Menunggu Pesanan</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-shipping-fast"></i></div>
                        <div class="tracking-step-label">Mengantar Pesanan</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-home"></i></div>
                        <div class="tracking-step-label">Pesanan Sampai</div>
                    </div>
                </div>
                
                <div class="estimated-time">
                    Estimasi Sampai: <span id="eta">30-45 menit</span>
                </div>
                
                <div class="tracking-map" id="map">
                    <!-- Peta akan ditampilkan di sini -->
                </div>
                
                <div class="driver-info">
                    <div class="driver-photo">
                        <i class="fas fa-user"></i>
                    </div>
                    <div class="driver-details">
                        <h4>Budi Santoso</h4>
                        <p>Driver GrabExpress • Honda Beat</p>
                        <p>Rating: ⭐⭐⭐⭐⭐ (4.9)</p>
                    </div>
                </div>
                
                <div class="tracking-info">
                    <h4>Detail Pesanan</h4>
                    <p><strong>No. Pesanan:</strong> HCM-2024-00123</p>
                    <p><strong>Waktu Pemesanan:</strong> 14:30 WIB</p>
                    <p><strong>Estimasi Sampai:</strong> 15:15 WIB</p>
                    <p><strong>Alamat Pengiriman:</strong> Jl. Merdeka No. 123, Jakarta</p>
                </div>
                
                <button class="btn" id="contact-driver">Hubungi Driver</button>
            </div>
        </div>
    </section>

    <!-- About Page -->
    <section class="page" id="about">
        <div class="container">
            <div class="section-title">
                <h2>Tentang Hanami Cafe</h2>
            </div>
            <div style="text-align: center; max-width: 800px; margin: 0 auto;">
                <p>Hanami Cafe terinspirasi dari tradisi Jepang menikmati keindahan bunga sakura. Kami menghadirkan suasana tenang dan damai di tengah hiruk pikuk kota, dengan menu kopi dan teh pilihan yang disajikan dengan teknik tradisional Jepang.</p>
                <p>Dibuka sejak 2020, Hanami Cafe telah menjadi tempat favorit bagi pecinta kopi dan teh yang mencari ketenangan dan kualitas terbaik.</p>
            </div>
        </div>
    </section>

    <!-- Contact Page -->
    <section class="page" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Hubungi Kami</h2>
            </div>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px;">
                <div>
                    <h3 style="margin-bottom: 20px; color: var(--primary);">Informasi Kontak</h3>
                    <p><i class="fas fa-map-marker-alt" style="margin-right: 10px;"></i> Jl. Sakura No. 123, Jakarta</p>
                    <p><i class="fas fa-phone" style="margin-right: 10px;"></i> (021) 1234-5678</p>
                    <p><i class="fas fa-envelope" style="margin-right: 10px;"></i> info@hanamicafe.com</p>
                    <p><i class="fas fa-clock" style="margin-right: 10px;"></i> Senin - Minggu: 07:00 - 22:00</p>
                </div>
                <div>
                    <h3 style="margin-bottom: 20px; color: var(--primary);">Kirim Pesan</h3>
                    <div class="form-group">
                        <input type="text" placeholder="Nama Anda">
                    </div>
                    <div class="form-group">
                        <input type="email" placeholder="Email Anda">
                    </div>
                    <div class="form-group">
                        <textarea rows="4" placeholder="Pesan Anda"></textarea>
                    </div>
                    <button class="btn">Kirim Pesan</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Cart Sidebar -->
    <div class="cart-sidebar" id="cart-sidebar">
        <div class="cart-header">
            <h3>Keranjang Belanja</h3>
            <button class="close-cart" id="close-cart">&times;</button>
        </div>
        <div class="cart-items" id="cart-items">
            <!-- Item keranjang akan ditampilkan di sini -->
        </div>
        <div class="cart-footer">
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">Rp 0</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Checkout</button>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Hanami Cafe</h3>
                    <p>Japanese Inspired Coffee & Tea. Nikmati pengalaman kopi dan teh Jepang yang autentik dengan sentuhan modern.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Link Cepat</h3>
                    <a href="#" class="nav-link" data-page="home">Beranda</a>
                    <a href="#" class="nav-link" data-page="menu">Menu</a>
                    <a href="#" class="nav-link" data-page="about">Tentang Kami</a>
                    <a href="#" class="nav-link" data-page="contact">Kontak</a>
                </div>
                <div class="footer-column">
                    <h3>Kontak</h3>
                    <p><i class="fas fa-map-marker-alt"></i> Jl. Sakura No. 123, Jakarta</p>
                    <p><i class="fas fa-phone"></i> (021) 1234-5678</p>
                    <p><i class="fas fa-envelope"></i> info@hanamicafe.com</p>
                </div>
                <div class="footer-column">
                    <h3>Jam Operasional</h3>
                    <p>Senin - Jumat: 07:00 - 22:00</p>
                    <p>Sabtu - Minggu: 08:00 - 23:00</p>
                </div>
            </div>
            <div class="copyright">
                &copy; 2023 Hanami Cafe. All rights reserved.
            </div>
        </div>
    </footer>

    <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>
    <script>
        // Data menu yang diperbarui
        const menuItems = [
            {
                id: 1,
                name: "Matcha Latte",
                category: "coffee",
                price: 35000,
                image: "https://images.unsplash.com/photo-1515823064-d6e0c04616a7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80",
                description: "Matcha premium dicampur dengan susu segar, memberikan rasa yang lembut dan nikmat. Matcha kami diimpor langsung dari Uji, Jepang."
            },
            {
                id: 2,
                name: "Sakura Tea",
                category: "tea",
                price: 28000,
                image: "https://images.unsplash.com/photo-1556679343-c7306c1976bc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80",
                description: "Teh sakura dengan aroma bunga yang khas, disajikan hangat atau dingin. Menggunakan kelopak sakura asli yang dapat dimakan."
            },
            {
                id: 3,
                name: "Dorayaki",
                category: "dessert",
                price: 25000,
                image: "https://images.unsplash.com/photo-1563729784474-d77dbb933a9e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Pancake Jepang dengan isian kacang merah manis, lembut dan lezat. Dapat ditambahkan es krim matcha sebagai topping."
            },
            {
                id: 4,
                name: "Ramen Special",
                category: "food",
                price: 45000,
                image: "https://images.unsplash.com/photo-1569718212165-3a8278d5f624?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1480&q=80",
                description: "Ramen dengan kaldu khusus dimasak selama 12 jam, dilengkapi chashu, telur ajitsuke, dan sayuran segar. Pilihan kurami: shoyu, miso, atau shio."
            },
            {
                id: 5,
                name: "Hojicha Latte",
                category: "coffee",
                price: 32000,
                image: "https://images.unsplash.com/photo-1571934811356-5cc061b6821f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1469&q=80",
                description: "Teh hojicha panggang dicampur dengan susu, rasa yang hangat dan comforting. Cocok untuk dinikmati di sore hari."
            },
            {
                id: 6,
                name: "Mochi Ice Cream",
                category: "dessert",
                price: 22000,
                image: "https://images.unsplash.com/photo-1603244307291-6d64e0fe0bb1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Es krim premium dibalut dengan mochi yang lembut, berbagai pilihan rasa: matcha, vanilla, stroberi, dan black sesame."
            },
            {
                id: 7,
                name: "Japanese Curry",
                category: "food",
                price: 38000,
                image: "https://images.unsplash.com/photo-1586190848861-99aa4a171e90?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1480&q=80",
                description: "Kari Jepang dengan tekstur yang kental dan rasa yang kaya, disajikan dengan nasi. Pilihan level pedas: mild, medium, atau hot."
            },
            {
                id: 8,
                name: "Genmaicha Tea",
                category: "tea",
                price: 26000,
                image: "https://images.unsplash.com/photo-1544787219-7f47ccb76574?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1392&q=80",
                description: "Teh hijau dicampur dengan beras panggang, aroma yang unik dan menenangkan. Dapat disajikan panas atau dingin."
            },
            {
                id: 9,
                name: "Mellon Bun",
                category: "dessert",
                price: 18000,
                image: "https://images.unsplash.com/photo-1555507036-ab794f27d2e9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Roti bun lembut dengan isian melon manis, tekstur yang fluffy dan rasa yang menyegarkan."
            },
            {
                id: 10,
                name: "Udon Special",
                category: "food",
                price: 42000,
                image: "https://images.unsplash.com/photo-1563245372-f21724e3856d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Udon dengan tekstur kenyal, disajikan dengan kaldu dashi yang gurih, tempura, dan sayuran segar."
            }
        ];

        // Harga topping dan perlengkapan
        const toppingPrices = {
            boba: 5000,
            grassjelly: 4000,
            pudding: 6000,
            cheese: 8000,
            onsen: 7000,
            utensils: 1500  // Perlengkapan wajib
        };

        // Biaya pengiriman dasar
        const baseDeliveryCost = 15000;
        const freeDeliveryThreshold = 75000;

        // State aplikasi
        let cart = [];
        let currentPage = 'home';
        let currentCategory = 'all';
        let currentItem = null;
        let currentCustomization = {
            sugar: 'normal',
            ice: 'normal',
            topping: null,
            utensils: 'utensils', // Wajib ada
            specialRequest: ''
        };

        // Koordinat Hanami Cafe (contoh: Jakarta)
        const hanamiCafeLocation = [-6.2088, 106.8456];

        // DOM Elements
        const cartIcon = document.getElementById('cart-icon');
        const cartSidebar = document.getElementById('cart-sidebar');
        const closeCart = document.getElementById('close-cart');
        const overlay = document.getElementById('overlay');
        const cartItems = document.getElementById('cart-items');
        const cartTotal = document.getElementById('cart-total');
        const cartCount = document.querySelector('.cart-count');
        const checkoutBtn = document.getElementById('checkout-btn');
        const backToCart = document.getElementById('back-to-cart');
        const confirmPayment = document.getElementById('confirm-payment');
        const paymentSummary = document.getElementById('payment-summary');
        const paymentTotal = document.getElementById('payment-total');
        const deliveryCost = document.getElementById('delivery-cost');
        const menuContainer = document.getElementById('menu-container');
        const homeMenuGrid = document.querySelector('#home .menu-grid');
        const categoryButtons = document.querySelectorAll('.category-btn');
        const navLinks = document.querySelectorAll('.nav-link');
        const pages = document.querySelectorAll('.page');
        const paymentMethods = document.querySelectorAll('.payment-method');
        const deliveryOptions = document.querySelectorAll('.delivery-option');
        const contactDriver = document.getElementById('contact-driver');

        // Form elements
        const nameInput = document.getElementById('name');
        const phoneInput = document.getElementById('phone');
        const emailInput = document.getElementById('email');
        const addressInput = document.getElementById('address');
        const notesInput = document.getElementById('notes');
        const charCount = document.getElementById('char-count');
        const notesCharCount = document.getElementById('notes-char-count');

        // Payment instruction elements
        const gopayInstructions = document.getElementById('gopay-instructions');
        const qrisInstructions = document.getElementById('qris-instructions');
        const vaInstructions = document.getElementById('va-instructions');
        const gopayAmount = document.getElementById('gopay-amount');
        const qrisAmount = document.getElementById('qris-amount');
        const vaAmount = document.getElementById('va-amount');

        // Modal Elements
        const itemModal = document.getElementById('item-modal');
        const modalClose = document.getElementById('modal-close');
        const modalImage = document.getElementById('modal-image');
        const modalTitle = document.getElementById('modal-title');
        const modalPrice = document.getElementById('modal-price');
        const modalDescription = document.getElementById('modal-description');
        const specialRequest = document.getElementById('special-request');
        const addToCartModal = document.getElementById('add-to-cart-modal');
        const qtyMinus = document.querySelector('.qty-minus');
        const qtyPlus = document.querySelector('.qty-plus');
        const qtyValue = document.querySelector('.qty-value');
        const optionItems = document.querySelectorAll('.option-item');

        // Format angka ke Rupiah
        function formatRupiah(angka) {
            return new Intl.NumberFormat('id-ID', {
                style: 'currency',
                currency: 'IDR',
                minimumFractionDigits: 0
            }).format(angka);
        }

        // Validasi form
        function validateForm() {
            let isValid = true;
            const errors = {};

            // Validasi nama
            if (!nameInput.value.trim()) {
                errors.name = 'Nama lengkap harus diisi';
                isValid = false;
            } else if (nameInput.value.trim().length > 20) {
                errors.name = 'Nama maksimal 20 karakter';
                isValid = false;
            }

            // Validasi telepon
            const phoneRegex = /^(\+62|62|0)8[1-9][0-9]{6,9}$/;
            if (!phoneInput.value.trim()) {
                errors.phone = 'Nomor telepon harus diisi';
                isValid = false;
            } else if (!phoneRegex.test(phoneInput.value.trim())) {
                errors.phone = 'Format nomor telepon tidak valid';
                isValid = false;
            }

            // Validasi email
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailInput.value.trim()) {
                errors.email = 'Email harus diisi';
                isValid = false;
            } else if (!emailRegex.test(emailInput.value.trim())) {
                errors.email = 'Format email tidak valid';
                isValid = false;
            }

            // Validasi alamat
            if (!addressInput.value.trim()) {
                errors.address = 'Alamat pengiriman harus diisi';
                isValid = false;
            }

            // Tampilkan error messages
            Object.keys(errors).forEach(field => {
                const errorElement = document.getElementById(`${field}-error`);
                const inputElement = document.getElementById(field);
                
                if (errorElement && inputElement) {
                    errorElement.textContent = errors[field];
                    inputElement.classList.toggle('error', !!errors[field]);
                }
            });

            // Hapus error messages untuk field yang valid
            ['name', 'phone', 'email', 'address'].forEach(field => {
                if (!errors[field]) {
                    const errorElement = document.getElementById(`${field}-error`);
                    const inputElement = document.getElementById(field);
                    
                    if (errorElement && inputElement) {
                        errorElement.textContent = '';
                        inputElement.classList.remove('error');
                    }
                }
            });

            return isValid;
        }

        // Kirim notifikasi ke penjual
        function sendSellerNotification(orderData) {
            // Simulasi pengiriman notifikasi email dan SMS
            console.log('Mengirim notifikasi ke penjual:');
            console.log('Email: order@hanamicafe.com');
            console.log('SMS: +6281917052090');
            console.log('Pesanan Baru:', orderData);
            
            // Dalam implementasi nyata, ini akan mengirim request ke API
            // fetch('/api/notify-seller', {
            //     method: 'POST',
            //     headers: { 'Content-Type': 'application/json' },
            //     body: JSON.stringify(orderData)
            // });
        }

        // Kirim notifikasi ke pelanggan
        function sendCustomerNotification(phone, message) {
            // Simulasi pengiriman SMS ke pelanggan
            console.log(`Mengirim SMS ke ${phone}: ${message}`);
            
            // Dalam implementasi nyata:
            // fetch('/api/send-sms', {
            //     method: 'POST',
            //     headers: { 'Content-Type': 'application/json' },
            //     body: JSON.stringify({ to: phone, message: message })
            // });
        }

        // Hitung biaya pengiriman berdasarkan jarak (simulasi)
        function calculateDeliveryCost(subtotal, address) {
            // Simulasi perhitungan jarak
            let distanceCost = baseDeliveryCost;
            
            // Dalam implementasi nyata, gunakan API seperti Google Maps Distance Matrix
            if (address.toLowerCase().includes('jakarta')) {
                distanceCost = baseDeliveryCost;
            } else if (address.toLowerCase().includes('bogor') || 
                      address.toLowerCase().includes('depok') || 
                      address.toLowerCase().includes('tangerang') || 
                      address.toLowerCase().includes('bekasi')) {
                distanceCost = baseDeliveryCost + 5000;
            } else {
                distanceCost = baseDeliveryCost + 10000;
            }
            
            // Gratis ongkir untuk order di atas threshold
            if (subtotal >= freeDeliveryThreshold) {
                return 0;
            }
            
            return distanceCost;
        }

        // Render menu items
        function renderMenuItems(container, items) {
            container.innerHTML = '';
            items.forEach(item => {
                const menuItem = document.createElement('div');
                menuItem.className = 'menu-item';
                menuItem.innerHTML = `
                    <img src="${item.image}" alt="${item.name}">
                    <div class="menu-item-content">
                        <h3>${item.name}</h3>
                        <p>${item.description}</p>
                        <div class="menu-item-price">
                            <span class="price">${formatRupiah(item.price)}</span>
                            <button class="add-to-cart" data-id="${item.id}">
                                <i class="fas fa-plus"></i>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(menuItem);
            });

            // Tambahkan event listener untuk tombol add to cart
            document.querySelectorAll('.add-to-cart').forEach(button => {
                button.addEventListener('click', function(e) {
                    e.stopPropagation();
                    const itemId = parseInt(this.getAttribute('data-id'));
                    addToCart(itemId);
                });
            });

            // Tambahkan event listener untuk item menu (modal detail)
            document.querySelectorAll('.menu-item').forEach(item => {
                item.addEventListener('click', function() {
                    const itemId = parseInt(this.querySelector('.add-to-cart').getAttribute('data-id'));
                    openItemModal(itemId);
                });
            });
        }

        // Buka modal detail item
        function openItemModal(itemId) {
            const item = menuItems.find(i => i.id === itemId);
            if (!item) return;
            
            currentItem = item;
            resetCustomization();
            
            modalImage.src = item.image;
            modalTitle.textContent = item.name;
            modalPrice.textContent = formatRupiah(item.price);
            modalDescription.textContent = item.description;
            qtyValue.textContent = '1';
            
            itemModal.classList.add('active');
            overlay.classList.add('active');
        }

        // Reset kustomisasi
        function resetCustomization() {
            currentCustomization = {
                sugar: 'normal',
                ice: 'normal',
                topping: null,
                utensils: 'utensils', // Wajib
                specialRequest: ''
            };
            
            // Reset UI
            optionItems.forEach(item => {
                item.classList.remove('selected');
            });
            
            // Set default selections
            document.querySelector('.option-item[data-value="normal"]').classList.add('selected');
            document.querySelector('.option-item[data-value="utensils"]').classList.add('selected');
            specialRequest.value = '';
            charCount.textContent = '0';
        }

        // Tambah item ke keranjang dengan kustomisasi
        function addToCart(itemId, quantity = 1) {
            const item = menuItems.find(i => i.id === itemId);
            if (!item) return;
            
            // Hitung harga dengan topping dan perlengkapan
            let finalPrice = item.price;
            if (currentCustomization.topping && toppingPrices[currentCustomization.topping]) {
                finalPrice += toppingPrices[currentCustomization.topping];
            }
            if (currentCustomization.utensils && toppingPrices[currentCustomization.utensils]) {
                finalPrice += toppingPrices[currentCustomization.utensils];
            }
            
            const cartItem = {
                ...item,
                finalPrice: finalPrice,
                quantity: quantity,
                customization: {...currentCustomization}
            };
            
            // Cek apakah item dengan kustomisasi yang sama sudah ada di keranjang
            const existingIndex = cart.findIndex(i => 
                i.id === itemId && 
                i.customization.sugar === currentCustomization.sugar &&
                i.customization.ice === currentCustomization.ice &&
                i.customization.topping === currentCustomization.topping &&
                i.customization.utensils === currentCustomization.utensils &&
                i.customization.specialRequest === currentCustomization.specialRequest
            );
            
            if (existingIndex !== -1) {
                cart[existingIndex].quantity += quantity;
            } else {
                cart.push(cartItem);
            }
            
            updateCart();
            showNotification(`${item.name} ditambahkan ke keranjang`);
            
            // Tutup modal jika terbuka
            if (itemModal.classList.contains('active')) {
                itemModal.classList.remove('active');
                overlay.classList.remove('active');
            }
        }

        // Hapus item dari keranjang
        function removeFromCart(itemIndex) {
            cart.splice(itemIndex, 1);
            updateCart();
        }

        // Update kuantitas item
        function updateQuantity(itemIndex, newQuantity) {
            if (newQuantity < 1) {
                removeFromCart(itemIndex);
                return;
            }
            
            cart[itemIndex].quantity = newQuantity;
            updateCart();
        }

        // Update tampilan keranjang
        function updateCart() {
            // Update jumlah item di icon keranjang
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            cartCount.textContent = totalItems;
            
            // Update daftar item di sidebar
            cartItems.innerHTML = '';
            let subtotal = 0;
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Keranjang belanja kosong</p>';
            } else {
                cart.forEach((item, index) => {
                    const itemTotal = item.finalPrice * item.quantity;
                    subtotal += itemTotal;
                    
                    const cartItem = document.createElement('div');
                    cartItem.className = 'cart-item';
                    
                    let customizationText = '';
                    if (item.customization.sugar !== 'normal') {
                        customizationText += `Gula: ${item.customization.sugar}, `;
                    }
                    if (item.customization.ice !== 'normal') {
                        customizationText += `Es: ${item.customization.ice}, `;
                    }
                    if (item.customization.topping) {
                        customizationText += `Topping: ${item.customization.topping}, `;
                    }
                    if (item.customization.utensils) {
                        customizationText += `Perlengkapan: Ya, `;
                    }
                    if (item.customization.specialRequest) {
                        customizationText += `Request: ${item.customization.specialRequest}`;
                    }
                    
                    // Hapus koma di akhir jika ada
                    if (customizationText.endsWith(', ')) {
                        customizationText = customizationText.slice(0, -2);
                    }
                    
                    cartItem.innerHTML = `
                        <img src="${item.image}" alt="${item.name}">
                        <div class="cart-item-details">
                            <h4>${item.name}</h4>
                            <div class="cart-item-price">${formatRupiah(item.finalPrice)}</div>
                            ${customizationText ? `<div class="cart-item-customization">${customizationText}</div>` : ''}
                            <div class="cart-item-quantity">
                                <button class="quantity-btn minus" data-index="${index}">-</button>
                                <span class="quantity">${item.quantity}</span>
                                <button class="quantity-btn plus" data-index="${index}">+</button>
                                <button class="remove-item" data-index="${index}"><i class="fas fa-trash"></i></button>
                            </div>
                        </div>
                    `;
                    cartItems.appendChild(cartItem);
                });
                
                // Tambahkan event listener untuk tombol kuantitas dan hapus
                document.querySelectorAll('.quantity-btn.minus').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        updateQuantity(itemIndex, cart[itemIndex].quantity - 1);
                    });
                });
                
                document.querySelectorAll('.quantity-btn.plus').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        updateQuantity(itemIndex, cart[itemIndex].quantity + 1);
                    });
                });
                
                document.querySelectorAll('.remove-item').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        removeFromCart(itemIndex);
                    });
                });
            }
            
            // Update total
            cartTotal.textContent = formatRupiah(subtotal);
            
            // Update ringkasan pembayaran
            updatePaymentSummary();
        }

        // Update ringkasan pembayaran
        function updatePaymentSummary() {
            paymentSummary.innerHTML = '';
            let subtotal = 0;
            
            cart.forEach(item => {
                const itemTotal = item.finalPrice * item.quantity;
                subtotal += itemTotal;
                
                const summaryItem = document.createElement('div');
                summaryItem.className = 'summary-item';
                summaryItem.innerHTML = `
                    <span>${item.name} x${item.quantity}</span>
                    <span>${formatRupiah(itemTotal)}</span>
                `;
                paymentSummary.appendChild(summaryItem);
            });
            
            // Hitung biaya pengiriman
            const delivery = calculateDeliveryCost(subtotal, addressInput.value);
            const total = subtotal + delivery;
            
            deliveryCost.textContent = formatRupiah(delivery);
            paymentTotal.textContent = formatRupiah(total);
            
            // Update jumlah pembayaran di semua metode
            gopayAmount.textContent = formatRupiah(total);
            qrisAmount.textContent = formatRupiah(total);
            vaAmount.textContent = formatRupiah(total);
        }

        // Tampilkan notifikasi
        function showNotification(message) {
            // Buat elemen notifikasi
            const notification = document.createElement('div');
            notification.style.cssText = `
                position: fixed;
                top: 20px;
                right: 20px;
                background-color: var(--primary);
                color: white;
                padding: 15px 20px;
                border-radius: 5px;
                box-shadow: 0 4px 8px rgba(0,0,0,0.2);
                z-index: 1001;
                transition: transform 0.3s, opacity 0.3s;
                transform: translateX(100%);
                opacity: 0;
            `;
            notification.textContent = message;
            document.body.appendChild(notification);
            
            // Animasi masuk
            setTimeout(() => {
                notification.style.transform = 'translateX(0)';
                notification.style.opacity = '1';
            }, 100);
            
            // Animasi keluar setelah 3 detik
            setTimeout(() => {
                notification.style.transform = 'translateX(100%)';
                notification.style.opacity = '0';
                setTimeout(() => {
                    document.body.removeChild(notification);
                }, 300);
            }, 3000);
        }

        // Filter menu berdasarkan kategori
        function filterMenu(category) {
            if (category === 'all') {
                return menuItems;
            }
            return menuItems.filter(item => item.category === category);
        }

        // Navigasi halaman
        function navigateToPage(page) {
            // Sembunyikan semua halaman
            pages.forEach(p => p.classList.remove('active'));
            
            // Tampilkan halaman yang dipilih
            document.getElementById(page).classList.add('active');
            
            // Update navigasi aktif
            navLinks.forEach(link => {
                if (link.getAttribute('data-page') === page) {
                    link.classList.add('active');
                } else {
                    link.classList.remove('active');
                }
            });
            
            // Tutup keranjang jika terbuka
            cartSidebar.classList.remove('active');
            overlay.classList.remove('active');
            
            currentPage = page;
            
            // Inisialisasi peta jika navigasi ke tracking page
            if (page === 'tracking') {
                initMap();
            }
        }

        // Inisialisasi peta tracking
        function initMap() {
            const map = L.map('map').setView(hanamiCafeLocation, 12);
            
            L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                attribution: '© OpenStreetMap contributors'
            }).addTo(map);
            
            // Tambahkan marker untuk Hanami Cafe
            L.marker(hanamiCafeLocation)
                .addTo(map)
                .bindPopup('Hanami Cafe')
                .openPopup();
            
            // Simulasi lokasi driver (random sekitar Jakarta)
            const driverLocation = [
                hanamiCafeLocation[0] + (Math.random() - 0.5) * 0.1,
                hanamiCafeLocation[1] + (Math.random() - 0.5) * 0.1
            ];
            
            L.marker(driverLocation)
                .addTo(map)
                .bindPopup('Driver Location')
                .openPopup();
        }

        // Inisialisasi aplikasi
        function init() {
            // Render menu di halaman home (hanya 4 item pertama)
            renderMenuItems(homeMenuGrid, menuItems.slice(0, 4));
            
            // Render menu di halaman menu
            renderMenuItems(menuContainer, menuItems);
            
            // Event listener untuk icon keranjang
            cartIcon.addEventListener('click', () => {
                cartSidebar.classList.add('active');
                overlay.classList.add('active');
            });
            
            // Event listener untuk tutup keranjang
            closeCart.addEventListener('click', () => {
                cartSidebar.classList.remove('active');
                overlay.classList.remove('active');
            });
            
            overlay.addEventListener('click', () => {
                cartSidebar.classList.remove('active');
                overlay.classList.remove('active');
                itemModal.classList.remove('active');
            });
            
            // Event listener untuk tombol checkout
            checkoutBtn.addEventListener('click', () => {
                if (cart.length === 0) {
                    showNotification('Keranjang belanja kosong');
                    return;
                }
                navigateToPage('payment');
            });
            
            // Event listener untuk kembali ke keranjang
            backToCart.addEventListener('click', () => {
                navigateToPage('menu');
                cartSidebar.classList.add('active');
                overlay.classList.add('active');
            });
            
            // Event listener untuk konfirmasi pembayaran
            confirmPayment.addEventListener('click', () => {
                if (cart.length === 0) {
                    showNotification('Keranjang belanja kosong');
                    return;
                }
                
                // Validasi form
                if (!validateForm()) {
                    showNotification('Harap lengkapi informasi pengiriman dengan benar');
                    return;
                }
                
                // Data pesanan
                const orderData = {
                    orderNumber: 'HCM-' + Date.now(),
                    customer: {
                        name: nameInput.value.trim(),
                        phone: phoneInput.value.trim(),
                        email: emailInput.value.trim(),
                        address: addressInput.value.trim(),
                        notes: notesInput.value.trim()
                    },
                    items: cart,
                    delivery: {
                        method: 'GrabExpress',
                        cost: calculateDeliveryCost(
                            cart.reduce((sum, item) => sum + (item.finalPrice * item.quantity), 0),
                            addressInput.value.trim()
                        )
                    },
                    total: parseFloat(paymentTotal.textContent.replace(/[^\d]/g, '')),
                    timestamp: new Date().toISOString()
                };
                
                // Kirim notifikasi ke penjual
                sendSellerNotification(orderData);
                
                // Kirim notifikasi ke pelanggan
                const customerMessage = `Terima kasih! Pesanan Anda di Hanami Cafe (${orderData.orderNumber}) telah diterima. Estimasi pengiriman: 30-45 menit.`;
                sendCustomerNotification(orderData.customer.phone, customerMessage);
                
                // Simulasi pembayaran berhasil
                showNotification('Pembayaran berhasil! Pesanan Anda sedang diproses.');
                
                // Reset keranjang dan form
                cart = [];
                updateCart();
                nameInput.value = '';
                phoneInput.value = '';
                emailInput.value = '';
                addressInput.value = '';
                notesInput.value = '';
                
                // Navigasi ke halaman tracking setelah 3 detik
                setTimeout(() => {
                    navigateToPage('tracking');
                }, 3000);
            });
            
            // Event listener untuk filter kategori
            categoryButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Update tombol aktif
                    categoryButtons.forEach(btn => btn.classList.remove('active'));
                    this.classList.add('active');
                    
                    // Filter menu
                    const category = this.getAttribute('data-category');
                    const filteredItems = filterMenu(category);
                    renderMenuItems(menuContainer, filteredItems);
                });
            });
            
            // Event listener untuk navigasi
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const page = this.getAttribute('data-page');
                    navigateToPage(page);
                });
            });
            
            // Event listener untuk metode pembayaran
            paymentMethods.forEach(method => {
                method.addEventListener('click', function() {
                    paymentMethods.forEach(m => m.classList.remove('selected'));
                    this.classList.add('selected');
                    
                    // Tampilkan instruksi pembayaran yang sesuai
                    const methodType = this.getAttribute('data-method');
                    gopayInstructions.classList.remove('active');
                    qrisInstructions.classList.remove('active');
                    vaInstructions.classList.remove('active');
                    
                    if (methodType === 'gopay') {
                        gopayInstructions.classList.add('active');
                    } else if (methodType === 'qris') {
                        qrisInstructions.classList.add('active');
                    } else if (methodType === 'va') {
                        vaInstructions.classList.add('active');
                    }
                });
            });
            
            // Event listener untuk pilihan pengiriman
            deliveryOptions.forEach(option => {
                option.addEventListener('click', function() {
                    deliveryOptions.forEach(o => o.classList.remove('selected'));
                    this.classList.add('selected');
                    updatePaymentSummary(); // Update biaya pengiriman
                });
            });
            
            // Event listener untuk hubungi driver
            contactDriver.addEventListener('click', () => {
                // Simulasi panggilan telepon
                window.open('tel:+6281234567890');
            });
            
            // Event listener untuk modal
            modalClose.addEventListener('click', () => {
                itemModal.classList.remove('active');
                overlay.classList.remove('active');
            });
            
            // Event listener untuk option items
            optionItems.forEach(item => {
                item.addEventListener('click', function() {
                    const group = this.parentElement;
                    const optionType = group.previousElementSibling.textContent.toLowerCase();
                    
                    // Untuk topping dan perlengkapan, bisa pilih multiple
                    if (optionType.includes('topping') || optionType.includes('perlengkapan')) {
                        this.classList.toggle('selected');
                    } else {
                        // Untuk yang lain, hanya satu pilihan
                        group.querySelectorAll('.option-item').forEach(i => {
                            i.classList.remove('selected');
                        });
                        this.classList.add('selected');
                    }
                    
                    // Update currentCustomization berdasarkan jenis option
                    if (optionType.includes('gula')) {
                        currentCustomization.sugar = this.getAttribute('data-value');
                    } else if (optionType.includes('es')) {
                        currentCustomization.ice = this.getAttribute('data-value');
                    } else if (optionType.includes('topping')) {
                        if (this.classList.contains('selected')) {
                            currentCustomization.topping = this.getAttribute('data-value');
                        } else {
                            currentCustomization.topping = null;
                        }
                    } else if (optionType.includes('perlengkapan')) {
                        currentCustomization.utensils = this.classList.contains('selected') ? 
                            this.getAttribute('data-value') : null;
                    }
                });
            });
            
            // Event listener untuk special request character count
            specialRequest.addEventListener('input', function() {
                currentCustomization.specialRequest = this.value;
                charCount.textContent = this.value.length;
            });
            
            // Event listener untuk notes character count
            notesInput.addEventListener('input', function() {
                notesCharCount.textContent = this.value.length;
            });
            
            // Event listener untuk alamat pengiriman (update ongkir real-time)
            addressInput.addEventListener('input', function() {
                updatePaymentSummary();
            });
            
            // Event listener untuk quantity selector
            qtyMinus.addEventListener('click', () => {
                let qty = parseInt(qtyValue.textContent);
                if (qty > 1) {
                    qtyValue.textContent = qty - 1;
                }
            });
            
            qtyPlus.addEventListener('click', () => {
                let qty = parseInt(qtyValue.textContent);
                qtyValue.textContent = qty + 1;
            });
            
            // Event listener untuk tambah ke keranjang dari modal
            addToCartModal.addEventListener('click', () => {
                if (currentItem) {
                    const quantity = parseInt(qtyValue.textContent);
                    addToCart(currentItem.id, quantity);
                }
            });
        }

        // Jalankan inisialisasi saat DOM siap
        document.addEventListener('DOMContentLoaded', init);
    </script>
</body>
</html><!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hanami Cafe - Japanese Inspired Coffee & Tea</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" />
    <style>
        /* Reset dan Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #8B4513;
            --secondary: #D4AF37;
            --accent: #C41E3A;
            --light: #F5F5DC;
            --dark: #3C2F2F;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background-color: var(--primary);
            color: white;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            color: var(--secondary);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 25px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            padding: 5px 10px;
            border-radius: 4px;
        }

        nav ul li a:hover {
            color: var(--secondary);
        }

        nav ul li a.active {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--secondary);
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 22px;
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: var(--accent);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: bold;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1554118811-1e0d58224f24?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1447&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            margin-bottom: 50px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto 30px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
        }

        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: var(--dark);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }

        .btn:hover {
            background-color: #e6c12e;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .btn:disabled {
            background-color: #ccc;
            cursor: not-allowed;
            transform: none;
        }

        /* Section Styles */
        section {
            padding: 60px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        .section-title h2 {
            font-size: 36px;
            color: var(--primary);
            display: inline-block;
            padding-bottom: 10px;
        }

        .section-title h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 3px;
            background-color: var(--secondary);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }

        /* Menu Section */
        .menu-categories {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .category-btn {
            background: none;
            border: 2px solid var(--primary);
            color: var(--primary);
            padding: 8px 20px;
            margin: 5px 10px;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
        }

        .category-btn.active, .category-btn:hover {
            background-color: var(--primary);
            color: white;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }

        .menu-item {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
            cursor: pointer;
        }

        .menu-item:hover {
            transform: translateY(-5px);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .menu-item-content {
            padding: 20px;
        }

        .menu-item h3 {
            font-size: 20px;
            margin-bottom: 10px;
            color: var(--primary);
        }

        .menu-item p {
            color: #666;
            margin-bottom: 15px;
            font-size: 14px;
        }

        .menu-item-price {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .price {
            font-weight: bold;
            color: var(--primary);
            font-size: 18px;
        }

        .add-to-cart {
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .add-to-cart:hover {
            background-color: var(--accent);
        }

        /* Modal Item Detail */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background-color: white;
            border-radius: 10px;
            max-width: 500px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
        }

        .modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: var(--dark);
            z-index: 1;
        }

        .modal-header {
            position: relative;
        }

        .modal-header img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 10px 10px 0 0;
        }

        .modal-body {
            padding: 20px;
        }

        .modal-title {
            font-size: 24px;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .modal-price {
            font-size: 20px;
            font-weight: bold;
            color: var(--primary);
            margin-bottom: 15px;
        }

        .modal-description {
            margin-bottom: 20px;
            color: #666;
        }

        .customization-options {
            margin-bottom: 20px;
        }

        .option-group {
            margin-bottom: 15px;
        }

        .option-title {
            font-weight: bold;
            margin-bottom: 8px;
            color: var(--dark);
        }

        .option-items {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .option-item {
            border: 1px solid #ddd;
            padding: 8px 15px;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 14px;
        }

        .option-item.selected {
            background-color: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .special-request {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-top: 10px;
            resize: vertical;
        }

        .char-count {
            font-size: 12px;
            color: #666;
            text-align: right;
            margin-top: 5px;
        }

        .modal-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .quantity-selector {
            display: flex;
            align-items: center;
        }

        .qty-btn {
            width: 35px;
            height: 35px;
            border: 1px solid #ddd;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 18px;
        }

        .qty-minus {
            border-radius: 5px 0 0 5px;
        }

        .qty-plus {
            border-radius: 0 5px 5px 0;
        }

        .qty-value {
            width: 50px;
            height: 35px;
            border-top: 1px solid #ddd;
            border-bottom: 1px solid #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* Cart Sidebar */
        .cart-sidebar {
            position: fixed;
            top: 0;
            right: -400px;
            width: 380px;
            height: 100vh;
            background-color: white;
            box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);
            transition: right 0.3s ease-in-out;
            z-index: 1000;
            display: flex;
            flex-direction: column;
        }

        .cart-sidebar.active {
            right: 0;
        }

        .cart-header {
            padding: 20px;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .cart-header h3 {
            color: var(--primary);
        }

        .close-cart {
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: #666;
        }

        .cart-items {
            flex: 1;
            overflow-y: auto;
            padding: 20px;
        }

        .cart-item {
            display: flex;
            margin-bottom: 15px;
            padding-bottom: 15px;
            border-bottom: 1px solid #eee;
        }

        .cart-item img {
            width: 80px;
            height: 80px;
            object-fit: cover;
            border-radius: 5px;
            margin-right: 15px;
        }

        .cart-item-details {
            flex: 1;
        }

        .cart-item-details h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }

        .cart-item-price {
            color: var(--dark);
            font-weight: bold;
            margin-bottom: 10px;
        }

        .cart-item-customization {
            font-size: 12px;
            color: #666;
            margin-bottom: 5px;
        }

        .cart-item-quantity {
            display: flex;
            align-items: center;
        }

        .quantity-btn {
            background-color: #f0f0f0;
            border: none;
            width: 25px;
            height: 25px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
        }

        .quantity {
            margin: 0 10px;
            font-weight: bold;
        }

        .remove-item {
            color: var(--accent);
            background: none;
            border: none;
            cursor: pointer;
            margin-left: 10px;
        }

        .cart-footer {
            padding: 20px;
            border-top: 1px solid #eee;
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            font-size: 18px;
            font-weight: bold;
        }

        .checkout-btn {
            width: 100%;
            padding: 12px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .checkout-btn:hover {
            background-color: var(--accent);
        }

        /* Payment Page */
        .payment-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .payment-steps {
            display: flex;
            justify-content: space-between;
            margin-bottom: 30px;
            position: relative;
        }

        .payment-steps:before {
            content: '';
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 2px;
            background-color: #eee;
            z-index: 1;
        }

        .step {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .step-number {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #eee;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 10px;
            font-weight: bold;
            color: #666;
        }

        .step.active .step-number {
            background-color: var(--primary);
            color: white;
        }

        .step.completed .step-number {
            background-color: var(--secondary);
            color: white;
        }

        .step-label {
            font-size: 14px;
            color: #666;
        }

        .step.active .step-label {
            color: var(--primary);
            font-weight: bold;
        }

        .payment-form {
            margin-bottom: 30px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .form-group input.error, .form-group textarea.error {
            border-color: var(--accent);
        }

        .error-message {
            color: var(--accent);
            font-size: 14px;
            margin-top: 5px;
        }

        .delivery-options {
            margin-bottom: 20px;
        }

        .delivery-option {
            border: 2px solid #eee;
            border-radius: 5px;
            padding: 15px;
            margin-bottom: 10px;
            cursor: pointer;
            transition: all 0.3s;
        }

        .delivery-option.selected {
            border-color: var(--primary);
            background-color: rgba(139, 69, 19, 0.05);
        }

        .delivery-option-header {
            display: flex;
            justify-content: between;
            align-items: center;
            margin-bottom: 10px;
        }

        .delivery-option-name {
            font-weight: bold;
            color: var(--primary);
        }

        .delivery-option-price {
            font-weight: bold;
        }

        .delivery-option-desc {
            font-size: 14px;
            color: #666;
        }

        .payment-methods {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-bottom: 30px;
        }

        .payment-method {
            border: 2px solid #eee;
            border-radius: 5px;
            padding: 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
        }

        .payment-method:hover, .payment-method.selected {
            border-color: var(--primary);
            background-color: rgba(139, 69, 19, 0.05);
        }

        .payment-method i {
            font-size: 30px;
            margin-bottom: 10px;
            color: var(--primary);
        }

        .payment-instructions {
            background-color: #f0f8ff;
            padding: 15px;
            border-radius: 5px;
            margin-top: 10px;
            display: none;
        }

        .payment-instructions.active {
            display: block;
        }

        .payment-instructions p {
            margin-bottom: 10px;
            font-size: 14px;
        }

        .qris-code {
            text-align: center;
            margin: 15px 0;
        }

        .qris-code img {
            max-width: 200px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .virtual-account {
            background-color: #e6f7ff;
            padding: 10px;
            border-radius: 5px;
            font-family: monospace;
            font-size: 16px;
            text-align: center;
            margin-bottom: 10px;
        }

        .order-summary {
            background-color: #f9f9f9;
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 30px;
        }

        .order-summary h3 {
            margin-bottom: 15px;
            color: var(--primary);
        }

        .summary-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }

        .summary-total {
            border-top: 1px solid #ddd;
            padding-top: 10px;
            margin-top: 10px;
            font-weight: bold;
            font-size: 18px;
        }

        .payment-actions {
            display: flex;
            justify-content: space-between;
        }

        .back-btn {
            background-color: #eee;
            color: #333;
        }

        .back-btn:hover {
            background-color: #ddd;
        }

        /* Tracking Page */
        .tracking-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .tracking-steps {
            display: flex;
            justify-content: space-between;
            margin: 40px 0;
            position: relative;
        }

        .tracking-steps:before {
            content: '';
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 3px;
            background-color: #eee;
            z-index: 1;
        }

        .tracking-step {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            z-index: 2;
            text-align: center;
        }

        .tracking-step-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #eee;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .tracking-step.active .tracking-step-icon {
            background-color: var(--primary);
            color: white;
        }

        .tracking-step.completed .tracking-step-icon {
            background-color: var(--secondary);
            color: white;
        }

        .tracking-step-label {
            font-size: 14px;
            font-weight: bold;
        }

        .tracking-info {
            background-color: #f9f9f9;
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 30px;
        }

        .tracking-map {
            height: 300px;
            background-color: #eee;
            border-radius: 5px;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .driver-info {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .driver-photo {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: #ddd;
            margin-right: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }

        .driver-details h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }

        .estimated-time {
            font-size: 18px;
            font-weight: bold;
            text-align: center;
            margin: 20px 0;
            color: var(--primary);
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-column h3 {
            font-size: 20px;
            margin-bottom: 20px;
            color: var(--secondary);
        }

        .footer-column p, .footer-column a {
            color: #ccc;
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-column a:hover {
            color: var(--secondary);
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-icons a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: background-color 0.3s;
        }

        .social-icons a:hover {
            background-color: var(--secondary);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #aaa;
            font-size: 14px;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
            
            .cart-sidebar {
                width: 100%;
                right: -100%;
            }
            
            .payment-methods {
                grid-template-columns: 1fr;
            }
            
            .modal-content {
                width: 95%;
            }
            
            .tracking-steps {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .tracking-steps:before {
                display: none;
            }
            
            .tracking-step {
                flex-direction: row;
                margin-bottom: 20px;
                width: 100%;
            }
            
            .tracking-step-icon {
                margin-right: 15px;
                margin-bottom: 0;
            }
        }

        /* Page Navigation */
        .page {
            display: none;
        }
        
        .page.active {
            display: block;
        }
        
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 999;
            display: none;
        }
        
        .overlay.active {
            display: block;
        }

        /* Map Container */
        #map {
            height: 300px;
            width: 100%;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <!-- Overlay untuk sidebar -->
    <div class="overlay" id="overlay"></div>

    <!-- Modal untuk detail item -->
    <div class="modal" id="item-modal">
        <div class="modal-content">
            <button class="modal-close" id="modal-close">&times;</button>
            <div class="modal-header">
                <img id="modal-image" src="" alt="">
            </div>
            <div class="modal-body">
                <h2 class="modal-title" id="modal-title"></h2>
                <div class="modal-price" id="modal-price"></div>
                <p class="modal-description" id="modal-description"></p>
                
                <div class="customization-options">
                    <div class="option-group">
                        <div class="option-title">Takaran Gula</div>
                        <div class="option-items">
                            <div class="option-item" data-value="normal">Normal</div>
                            <div class="option-item" data-value="less">Kurang Manis</div>
                            <div class="option-item" data-value="none">Tanpa Gula</div>
                            <div class="option-item" data-value="extra">Extra Manis</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Takaran Es</div>
                        <div class="option-items">
                            <div class="option-item" data-value="normal">Normal</div>
                            <div class="option-item" data-value="less">Kurang Es</div>
                            <div class="option-item" data-value="none">Tanpa Es</div>
                            <div class="option-item" data-value="extra">Extra Es</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Additional Topping</div>
                        <div class="option-items">
                            <div class="option-item" data-value="boba">Boba (+Rp 5,000)</div>
                            <div class="option-item" data-value="grassjelly">Grass Jelly (+Rp 4,000)</div>
                            <div class="option-item" data-value="pudding">Pudding (+Rp 6,000)</div>
                            <div class="option-item" data-value="cheese">Cheese Foam (+Rp 8,000)</div>
                            <div class="option-item" data-value="onsen">Onsen Tamago (+Rp 7,000)</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Perlengkapan Wajib*</div>
                        <div class="option-items">
                            <div class="option-item selected" data-value="utensils">Sendok & Garpu/Sumpit (+Rp 1,500)</div>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <div class="option-title">Request Khusus</div>
                        <textarea class="special-request" id="special-request" placeholder="Contoh: Susu almond, ekstra hot, dll." maxlength="80"></textarea>
                        <div class="char-count"><span id="char-count">0</span>/80 karakter</div>
                    </div>
                </div>
                
                <div class="modal-actions">
                    <div class="quantity-selector">
                        <button class="qty-btn qty-minus">-</button>
                        <div class="qty-value">1</div>
                        <button class="qty-btn qty-plus">+</button>
                    </div>
                    <button class="btn" id="add-to-cart-modal">Tambah ke Keranjang</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <i class="fas fa-leaf"></i>
                <span>Hanami Cafe</span>
            </div>
            <nav>
                <ul>
                    <li><a href="#" class="nav-link active" data-page="home">Beranda</a></li>
                    <li><a href="#" class="nav-link" data-page="menu">Menu</a></li>
                    <li><a href="#" class="nav-link" data-page="about">Tentang Kami</a></li>
                    <li><a href="#" class="nav-link" data-page="contact">Kontak</a></li>
                </ul>
            </nav>
            <div class="cart-icon" id="cart-icon">
                <i class="fas fa-shopping-cart"></i>
                <span class="cart-count">0</span>
            </div>
        </div>
    </header>

    <!-- Home Page -->
    <section class="page active" id="home">
        <div class="hero">
            <h1>Selamat Datang di Hanami Cafe</h1>
            <p>Nikmati pengalaman kopi dan teh Jepang yang autentik dengan sentuhan modern di tengah suasana yang menenangkan.</p>
            <a href="#" class="btn nav-link" data-page="menu">Lihat Menu</a>
        </div>

        <div class="container">
            <div class="section-title">
                <h2>Menu Spesial Kami</h2>
            </div>
            <div class="menu-grid">
                <!-- Item menu akan ditampilkan di sini -->
            </div>
        </div>
    </section>

    <!-- Menu Page -->
    <section class="page" id="menu">
        <div class="container">
            <div class="section-title">
                <h2>Menu Lengkap</h2>
            </div>
            
            <div class="menu-categories">
                <button class="category-btn active" data-category="all">Semua</button>
                <button class="category-btn" data-category="coffee">Kopi</button>
                <button class="category-btn" data-category="tea">Teh</button>
                <button class="category-btn" data-category="dessert">Dessert</button>
                <button class="category-btn" data-category="food">Makanan</button>
            </div>
            
            <div class="menu-grid" id="menu-container">
                <!-- Item menu akan ditampilkan di sini -->
            </div>
        </div>
    </section>

    <!-- Payment Page -->
    <section class="page" id="payment">
        <div class="container">
            <div class="section-title">
                <h2>Checkout</h2>
            </div>
            
            <div class="payment-container">
                <div class="payment-steps">
                    <div class="step completed">
                        <div class="step-number">1</div>
                        <div class="step-label">Keranjang</div>
                    </div>
                    <div class="step active">
                        <div class="step-number">2</div>
                        <div class="step-label">Pembayaran</div>
                    </div>
                    <div class="step">
                        <div class="step-number">3</div>
                        <div class="step-label">Selesai</div>
                    </div>
                </div>
                
                <div class="payment-form">
                    <h3>Informasi Pengiriman</h3>
                    <div class="form-group">
                        <label for="name">Nama Lengkap *</label>
                        <input type="text" id="name" placeholder="Masukkan nama lengkap (maks. 20 huruf)" maxlength="20">
                        <div class="error-message" id="name-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="phone">Nomor Telepon *</label>
                        <input type="tel" id="phone" placeholder="Contoh: 081234567890">
                        <div class="error-message" id="phone-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="email">Email *</label>
                        <input type="email" id="email" placeholder="email@contoh.com">
                        <div class="error-message" id="email-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="address">Alamat Pengiriman *</label>
                        <textarea id="address" rows="3" placeholder="Masukkan alamat lengkap"></textarea>
                        <div class="error-message" id="address-error"></div>
                    </div>
                    <div class="form-group">
                        <label for="notes">Catatan (opsional, maks. 80 huruf)</label>
                        <textarea id="notes" rows="2" placeholder="Catatan khusus untuk pesanan" maxlength="80"></textarea>
                        <div class="char-count"><span id="notes-char-count">0</span>/80 karakter</div>
                    </div>
                </div>
                
                <h3>Pilihan Pengiriman</h3>
                <div class="delivery-options">
                    <div class="delivery-option selected" data-delivery="grabexpress">
                        <div class="delivery-option-header">
                            <span class="delivery-option-name">GrabExpress</span>
                            <span class="delivery-option-price" id="delivery-price">Rp 15,000</span>
                        </div>
                        <div class="delivery-option-desc">Estimasi: 30-45 menit • Gratis ongkir untuk order di atas Rp 75,000</div>
                    </div>
                </div>
                
                <h3>Metode Pembayaran</h3>
                <div class="payment-methods">
                    <div class="payment-method selected" data-method="gopay">
                        <i class="fas fa-wallet"></i>
                        <div>Gopay</div>
                    </div>
                    <div class="payment-method" data-method="qris">
                        <i class="fas fa-qrcode"></i>
                        <div>QRIS</div>
                    </div>
                    <div class="payment-method" data-method="va">
                        <i class="fas fa-university"></i>
                        <div>Virtual Account</div>
                    </div>
                </div>
                
                <!-- Instruksi Pembayaran -->
                <div class="payment-instructions active" id="gopay-instructions">
                    <p><strong>Instruksi Pembayaran Gopay:</strong></p>
                    <p>1. Buka aplikasi Gopay di smartphone Anda</p>
                    <p>2. Pilih "Bayar" dan scan QR code berikut</p>
                    <div class="qris-code">
                        <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=HANAMICAFE-ORDER-2024" alt="QR Code Gopay">
                    </div>
                    <p>3. Atau gunakan nomor virtual berikut: <strong>8080801234567890</strong></p>
                    <p>4. Jumlah yang harus dibayar: <strong id="gopay-amount">Rp 0</strong></p>
                </div>
                
                <div class="payment-instructions" id="qris-instructions">
                    <p><strong>Instruksi Pembayaran QRIS:</strong></p>
                    <p>1. Buka aplikasi e-wallet atau mobile banking Anda</p>
                    <p>2. Pilih fitur "Scan QRIS"</p>
                    <p>3. Scan QR code berikut</p>
                    <div class="qris-code">
                        <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=HANAMICAFE-QRIS-ORDER-2024" alt="QR Code QRIS">
                    </div>
                    <p>4. Jumlah yang harus dibayar: <strong id="qris-amount">Rp 0</strong></p>
                </div>
                
                <div class="payment-instructions" id="va-instructions">
                    <p><strong>Instruksi Pembayaran Virtual Account:</strong></p>
                    <p>1. Buka aplikasi mobile banking Anda</p>
                    <p>2. Pilih "Transfer" → "Virtual Account"</p>
                    <p>3. Masukkan nomor virtual account berikut:</p>
                    <div class="virtual-account">8080801234567890</div>
                    <p>4. Jumlah yang harus dibayar: <strong id="va-amount">Rp 0</strong></p>
                    <p>5. Transaksi akan diproses otomatis</p>
                </div>
                
                <div class="order-summary">
                    <h3>Ringkasan Pesanan</h3>
                    <div id="payment-summary">
                        <!-- Item pesanan akan ditampilkan di sini -->
                    </div>
                    <div class="summary-item">
                        <span>Ongkos Kirim</span>
                        <span id="delivery-cost">Rp 15,000</span>
                    </div>
                    <div class="summary-item summary-total">
                        <span>Total</span>
                        <span id="payment-total">Rp 0</span>
                    </div>
                </div>
                
                <div class="payment-actions">
                    <button class="btn back-btn" id="back-to-cart">Kembali ke Keranjang</button>
                    <button class="btn" id="confirm-payment">Bayar Sekarang</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Tracking Page -->
    <section class="page" id="tracking">
        <div class="container">
            <div class="section-title">
                <h2>Lacak Pesanan Anda</h2>
            </div>
            
            <div class="tracking-container">
                <div class="tracking-steps">
                    <div class="tracking-step completed">
                        <div class="tracking-step-icon"><i class="fas fa-utensils"></i></div>
                        <div class="tracking-step-label">Pesanan Diproses</div>
                    </div>
                    <div class="tracking-step active">
                        <div class="tracking-step-icon"><i class="fas fa-motorcycle"></i></div>
                        <div class="tracking-step-label">Driver Menuju Cafe</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-coffee"></i></div>
                        <div class="tracking-step-label">Menunggu Pesanan</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-shipping-fast"></i></div>
                        <div class="tracking-step-label">Mengantar Pesanan</div>
                    </div>
                    <div class="tracking-step">
                        <div class="tracking-step-icon"><i class="fas fa-home"></i></div>
                        <div class="tracking-step-label">Pesanan Sampai</div>
                    </div>
                </div>
                
                <div class="estimated-time">
                    Estimasi Sampai: <span id="eta">30-45 menit</span>
                </div>
                
                <div class="tracking-map" id="map">
                    <!-- Peta akan ditampilkan di sini -->
                </div>
                
                <div class="driver-info">
                    <div class="driver-photo">
                        <i class="fas fa-user"></i>
                    </div>
                    <div class="driver-details">
                        <h4>Budi Santoso</h4>
                        <p>Driver GrabExpress • Honda Beat</p>
                        <p>Rating: ⭐⭐⭐⭐⭐ (4.9)</p>
                    </div>
                </div>
                
                <div class="tracking-info">
                    <h4>Detail Pesanan</h4>
                    <p><strong>No. Pesanan:</strong> HCM-2024-00123</p>
                    <p><strong>Waktu Pemesanan:</strong> 14:30 WIB</p>
                    <p><strong>Estimasi Sampai:</strong> 15:15 WIB</p>
                    <p><strong>Alamat Pengiriman:</strong> Jl. Merdeka No. 123, Jakarta</p>
                </div>
                
                <button class="btn" id="contact-driver">Hubungi Driver</button>
            </div>
        </div>
    </section>

    <!-- About Page -->
    <section class="page" id="about">
        <div class="container">
            <div class="section-title">
                <h2>Tentang Hanami Cafe</h2>
            </div>
            <div style="text-align: center; max-width: 800px; margin: 0 auto;">
                <p>Hanami Cafe terinspirasi dari tradisi Jepang menikmati keindahan bunga sakura. Kami menghadirkan suasana tenang dan damai di tengah hiruk pikuk kota, dengan menu kopi dan teh pilihan yang disajikan dengan teknik tradisional Jepang.</p>
                <p>Dibuka sejak 2020, Hanami Cafe telah menjadi tempat favorit bagi pecinta kopi dan teh yang mencari ketenangan dan kualitas terbaik.</p>
            </div>
        </div>
    </section>

    <!-- Contact Page -->
    <section class="page" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Hubungi Kami</h2>
            </div>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px;">
                <div>
                    <h3 style="margin-bottom: 20px; color: var(--primary);">Informasi Kontak</h3>
                    <p><i class="fas fa-map-marker-alt" style="margin-right: 10px;"></i> Jl. Sakura No. 123, Jakarta</p>
                    <p><i class="fas fa-phone" style="margin-right: 10px;"></i> (021) 1234-5678</p>
                    <p><i class="fas fa-envelope" style="margin-right: 10px;"></i> info@hanamicafe.com</p>
                    <p><i class="fas fa-clock" style="margin-right: 10px;"></i> Senin - Minggu: 07:00 - 22:00</p>
                </div>
                <div>
                    <h3 style="margin-bottom: 20px; color: var(--primary);">Kirim Pesan</h3>
                    <div class="form-group">
                        <input type="text" placeholder="Nama Anda">
                    </div>
                    <div class="form-group">
                        <input type="email" placeholder="Email Anda">
                    </div>
                    <div class="form-group">
                        <textarea rows="4" placeholder="Pesan Anda"></textarea>
                    </div>
                    <button class="btn">Kirim Pesan</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Cart Sidebar -->
    <div class="cart-sidebar" id="cart-sidebar">
        <div class="cart-header">
            <h3>Keranjang Belanja</h3>
            <button class="close-cart" id="close-cart">&times;</button>
        </div>
        <div class="cart-items" id="cart-items">
            <!-- Item keranjang akan ditampilkan di sini -->
        </div>
        <div class="cart-footer">
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">Rp 0</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Checkout</button>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Hanami Cafe</h3>
                    <p>Japanese Inspired Coffee & Tea. Nikmati pengalaman kopi dan teh Jepang yang autentik dengan sentuhan modern.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Link Cepat</h3>
                    <a href="#" class="nav-link" data-page="home">Beranda</a>
                    <a href="#" class="nav-link" data-page="menu">Menu</a>
                    <a href="#" class="nav-link" data-page="about">Tentang Kami</a>
                    <a href="#" class="nav-link" data-page="contact">Kontak</a>
                </div>
                <div class="footer-column">
                    <h3>Kontak</h3>
                    <p><i class="fas fa-map-marker-alt"></i> Jl. Sakura No. 123, Jakarta</p>
                    <p><i class="fas fa-phone"></i> (021) 1234-5678</p>
                    <p><i class="fas fa-envelope"></i> info@hanamicafe.com</p>
                </div>
                <div class="footer-column">
                    <h3>Jam Operasional</h3>
                    <p>Senin - Jumat: 07:00 - 22:00</p>
                    <p>Sabtu - Minggu: 08:00 - 23:00</p>
                </div>
            </div>
            <div class="copyright">
                &copy; 2023 Hanami Cafe. All rights reserved.
            </div>
        </div>
    </footer>

    <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>
    <script>
        // Data menu yang diperbarui
        const menuItems = [
            {
                id: 1,
                name: "Matcha Latte",
                category: "coffee",
                price: 35000,
                image: "https://images.unsplash.com/photo-1515823064-d6e0c04616a7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80",
                description: "Matcha premium dicampur dengan susu segar, memberikan rasa yang lembut dan nikmat. Matcha kami diimpor langsung dari Uji, Jepang."
            },
            {
                id: 2,
                name: "Sakura Tea",
                category: "tea",
                price: 28000,
                image: "https://images.unsplash.com/photo-1556679343-c7306c1976bc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80",
                description: "Teh sakura dengan aroma bunga yang khas, disajikan hangat atau dingin. Menggunakan kelopak sakura asli yang dapat dimakan."
            },
            {
                id: 3,
                name: "Dorayaki",
                category: "dessert",
                price: 25000,
                image: "https://images.unsplash.com/photo-1563729784474-d77dbb933a9e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Pancake Jepang dengan isian kacang merah manis, lembut dan lezat. Dapat ditambahkan es krim matcha sebagai topping."
            },
            {
                id: 4,
                name: "Ramen Special",
                category: "food",
                price: 45000,
                image: "https://images.unsplash.com/photo-1569718212165-3a8278d5f624?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1480&q=80",
                description: "Ramen dengan kaldu khusus dimasak selama 12 jam, dilengkapi chashu, telur ajitsuke, dan sayuran segar. Pilihan kurami: shoyu, miso, atau shio."
            },
            {
                id: 5,
                name: "Hojicha Latte",
                category: "coffee",
                price: 32000,
                image: "https://images.unsplash.com/photo-1571934811356-5cc061b6821f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1469&q=80",
                description: "Teh hojicha panggang dicampur dengan susu, rasa yang hangat dan comforting. Cocok untuk dinikmati di sore hari."
            },
            {
                id: 6,
                name: "Mochi Ice Cream",
                category: "dessert",
                price: 22000,
                image: "https://images.unsplash.com/photo-1603244307291-6d64e0fe0bb1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Es krim premium dibalut dengan mochi yang lembut, berbagai pilihan rasa: matcha, vanilla, stroberi, dan black sesame."
            },
            {
                id: 7,
                name: "Japanese Curry",
                category: "food",
                price: 38000,
                image: "https://images.unsplash.com/photo-1586190848861-99aa4a171e90?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1480&q=80",
                description: "Kari Jepang dengan tekstur yang kental dan rasa yang kaya, disajikan dengan nasi. Pilihan level pedas: mild, medium, atau hot."
            },
            {
                id: 8,
                name: "Genmaicha Tea",
                category: "tea",
                price: 26000,
                image: "https://images.unsplash.com/photo-1544787219-7f47ccb76574?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1392&q=80",
                description: "Teh hijau dicampur dengan beras panggang, aroma yang unik dan menenangkan. Dapat disajikan panas atau dingin."
            },
            {
                id: 9,
                name: "Mellon Bun",
                category: "dessert",
                price: 18000,
                image: "https://images.unsplash.com/photo-1555507036-ab794f27d2e9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Roti bun lembut dengan isian melon manis, tekstur yang fluffy dan rasa yang menyegarkan."
            },
            {
                id: 10,
                name: "Udon Special",
                category: "food",
                price: 42000,
                image: "https://images.unsplash.com/photo-1563245372-f21724e3856d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80",
                description: "Udon dengan tekstur kenyal, disajikan dengan kaldu dashi yang gurih, tempura, dan sayuran segar."
            }
        ];

        // Harga topping dan perlengkapan
        const toppingPrices = {
            boba: 5000,
            grassjelly: 4000,
            pudding: 6000,
            cheese: 8000,
            onsen: 7000,
            utensils: 1500  // Perlengkapan wajib
        };

        // Biaya pengiriman dasar
        const baseDeliveryCost = 15000;
        const freeDeliveryThreshold = 75000;

        // State aplikasi
        let cart = [];
        let currentPage = 'home';
        let currentCategory = 'all';
        let currentItem = null;
        let currentCustomization = {
            sugar: 'normal',
            ice: 'normal',
            topping: null,
            utensils: 'utensils', // Wajib ada
            specialRequest: ''
        };

        // Koordinat Hanami Cafe (contoh: Jakarta)
        const hanamiCafeLocation = [-6.2088, 106.8456];

        // DOM Elements
        const cartIcon = document.getElementById('cart-icon');
        const cartSidebar = document.getElementById('cart-sidebar');
        const closeCart = document.getElementById('close-cart');
        const overlay = document.getElementById('overlay');
        const cartItems = document.getElementById('cart-items');
        const cartTotal = document.getElementById('cart-total');
        const cartCount = document.querySelector('.cart-count');
        const checkoutBtn = document.getElementById('checkout-btn');
        const backToCart = document.getElementById('back-to-cart');
        const confirmPayment = document.getElementById('confirm-payment');
        const paymentSummary = document.getElementById('payment-summary');
        const paymentTotal = document.getElementById('payment-total');
        const deliveryCost = document.getElementById('delivery-cost');
        const menuContainer = document.getElementById('menu-container');
        const homeMenuGrid = document.querySelector('#home .menu-grid');
        const categoryButtons = document.querySelectorAll('.category-btn');
        const navLinks = document.querySelectorAll('.nav-link');
        const pages = document.querySelectorAll('.page');
        const paymentMethods = document.querySelectorAll('.payment-method');
        const deliveryOptions = document.querySelectorAll('.delivery-option');
        const contactDriver = document.getElementById('contact-driver');

        // Form elements
        const nameInput = document.getElementById('name');
        const phoneInput = document.getElementById('phone');
        const emailInput = document.getElementById('email');
        const addressInput = document.getElementById('address');
        const notesInput = document.getElementById('notes');
        const charCount = document.getElementById('char-count');
        const notesCharCount = document.getElementById('notes-char-count');

        // Payment instruction elements
        const gopayInstructions = document.getElementById('gopay-instructions');
        const qrisInstructions = document.getElementById('qris-instructions');
        const vaInstructions = document.getElementById('va-instructions');
        const gopayAmount = document.getElementById('gopay-amount');
        const qrisAmount = document.getElementById('qris-amount');
        const vaAmount = document.getElementById('va-amount');

        // Modal Elements
        const itemModal = document.getElementById('item-modal');
        const modalClose = document.getElementById('modal-close');
        const modalImage = document.getElementById('modal-image');
        const modalTitle = document.getElementById('modal-title');
        const modalPrice = document.getElementById('modal-price');
        const modalDescription = document.getElementById('modal-description');
        const specialRequest = document.getElementById('special-request');
        const addToCartModal = document.getElementById('add-to-cart-modal');
        const qtyMinus = document.querySelector('.qty-minus');
        const qtyPlus = document.querySelector('.qty-plus');
        const qtyValue = document.querySelector('.qty-value');
        const optionItems = document.querySelectorAll('.option-item');

        // Format angka ke Rupiah
        function formatRupiah(angka) {
            return new Intl.NumberFormat('id-ID', {
                style: 'currency',
                currency: 'IDR',
                minimumFractionDigits: 0
            }).format(angka);
        }

        // Validasi form
        function validateForm() {
            let isValid = true;
            const errors = {};

            // Validasi nama
            if (!nameInput.value.trim()) {
                errors.name = 'Nama lengkap harus diisi';
                isValid = false;
            } else if (nameInput.value.trim().length > 20) {
                errors.name = 'Nama maksimal 20 karakter';
                isValid = false;
            }

            // Validasi telepon
            const phoneRegex = /^(\+62|62|0)8[1-9][0-9]{6,9}$/;
            if (!phoneInput.value.trim()) {
                errors.phone = 'Nomor telepon harus diisi';
                isValid = false;
            } else if (!phoneRegex.test(phoneInput.value.trim())) {
                errors.phone = 'Format nomor telepon tidak valid';
                isValid = false;
            }

            // Validasi email
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailInput.value.trim()) {
                errors.email = 'Email harus diisi';
                isValid = false;
            } else if (!emailRegex.test(emailInput.value.trim())) {
                errors.email = 'Format email tidak valid';
                isValid = false;
            }

            // Validasi alamat
            if (!addressInput.value.trim()) {
                errors.address = 'Alamat pengiriman harus diisi';
                isValid = false;
            }

            // Tampilkan error messages
            Object.keys(errors).forEach(field => {
                const errorElement = document.getElementById(`${field}-error`);
                const inputElement = document.getElementById(field);
                
                if (errorElement && inputElement) {
                    errorElement.textContent = errors[field];
                    inputElement.classList.toggle('error', !!errors[field]);
                }
            });

            // Hapus error messages untuk field yang valid
            ['name', 'phone', 'email', 'address'].forEach(field => {
                if (!errors[field]) {
                    const errorElement = document.getElementById(`${field}-error`);
                    const inputElement = document.getElementById(field);
                    
                    if (errorElement && inputElement) {
                        errorElement.textContent = '';
                        inputElement.classList.remove('error');
                    }
                }
            });

            return isValid;
        }

        // Kirim notifikasi ke penjual
        function sendSellerNotification(orderData) {
            // Simulasi pengiriman notifikasi email dan SMS
            console.log('Mengirim notifikasi ke penjual:');
            console.log('Email: order@hanamicafe.com');
            console.log('SMS: +6281917052090');
            console.log('Pesanan Baru:', orderData);
            
            // Dalam implementasi nyata, ini akan mengirim request ke API
            // fetch('/api/notify-seller', {
            //     method: 'POST',
            //     headers: { 'Content-Type': 'application/json' },
            //     body: JSON.stringify(orderData)
            // });
        }

        // Kirim notifikasi ke pelanggan
        function sendCustomerNotification(phone, message) {
            // Simulasi pengiriman SMS ke pelanggan
            console.log(`Mengirim SMS ke ${phone}: ${message}`);
            
            // Dalam implementasi nyata:
            // fetch('/api/send-sms', {
            //     method: 'POST',
            //     headers: { 'Content-Type': 'application/json' },
            //     body: JSON.stringify({ to: phone, message: message })
            // });
        }

        // Hitung biaya pengiriman berdasarkan jarak (simulasi)
        function calculateDeliveryCost(subtotal, address) {
            // Simulasi perhitungan jarak
            let distanceCost = baseDeliveryCost;
            
            // Dalam implementasi nyata, gunakan API seperti Google Maps Distance Matrix
            if (address.toLowerCase().includes('jakarta')) {
                distanceCost = baseDeliveryCost;
            } else if (address.toLowerCase().includes('bogor') || 
                      address.toLowerCase().includes('depok') || 
                      address.toLowerCase().includes('tangerang') || 
                      address.toLowerCase().includes('bekasi')) {
                distanceCost = baseDeliveryCost + 5000;
            } else {
                distanceCost = baseDeliveryCost + 10000;
            }
            
            // Gratis ongkir untuk order di atas threshold
            if (subtotal >= freeDeliveryThreshold) {
                return 0;
            }
            
            return distanceCost;
        }

        // Render menu items
        function renderMenuItems(container, items) {
            container.innerHTML = '';
            items.forEach(item => {
                const menuItem = document.createElement('div');
                menuItem.className = 'menu-item';
                menuItem.innerHTML = `
                    <img src="${item.image}" alt="${item.name}">
                    <div class="menu-item-content">
                        <h3>${item.name}</h3>
                        <p>${item.description}</p>
                        <div class="menu-item-price">
                            <span class="price">${formatRupiah(item.price)}</span>
                            <button class="add-to-cart" data-id="${item.id}">
                                <i class="fas fa-plus"></i>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(menuItem);
            });

            // Tambahkan event listener untuk tombol add to cart
            document.querySelectorAll('.add-to-cart').forEach(button => {
                button.addEventListener('click', function(e) {
                    e.stopPropagation();
                    const itemId = parseInt(this.getAttribute('data-id'));
                    addToCart(itemId);
                });
            });

            // Tambahkan event listener untuk item menu (modal detail)
            document.querySelectorAll('.menu-item').forEach(item => {
                item.addEventListener('click', function() {
                    const itemId = parseInt(this.querySelector('.add-to-cart').getAttribute('data-id'));
                    openItemModal(itemId);
                });
            });
        }

        // Buka modal detail item
        function openItemModal(itemId) {
            const item = menuItems.find(i => i.id === itemId);
            if (!item) return;
            
            currentItem = item;
            resetCustomization();
            
            modalImage.src = item.image;
            modalTitle.textContent = item.name;
            modalPrice.textContent = formatRupiah(item.price);
            modalDescription.textContent = item.description;
            qtyValue.textContent = '1';
            
            itemModal.classList.add('active');
            overlay.classList.add('active');
        }

        // Reset kustomisasi
        function resetCustomization() {
            currentCustomization = {
                sugar: 'normal',
                ice: 'normal',
                topping: null,
                utensils: 'utensils', // Wajib
                specialRequest: ''
            };
            
            // Reset UI
            optionItems.forEach(item => {
                item.classList.remove('selected');
            });
            
            // Set default selections
            document.querySelector('.option-item[data-value="normal"]').classList.add('selected');
            document.querySelector('.option-item[data-value="utensils"]').classList.add('selected');
            specialRequest.value = '';
            charCount.textContent = '0';
        }

        // Tambah item ke keranjang dengan kustomisasi
        function addToCart(itemId, quantity = 1) {
            const item = menuItems.find(i => i.id === itemId);
            if (!item) return;
            
            // Hitung harga dengan topping dan perlengkapan
            let finalPrice = item.price;
            if (currentCustomization.topping && toppingPrices[currentCustomization.topping]) {
                finalPrice += toppingPrices[currentCustomization.topping];
            }
            if (currentCustomization.utensils && toppingPrices[currentCustomization.utensils]) {
                finalPrice += toppingPrices[currentCustomization.utensils];
            }
            
            const cartItem = {
                ...item,
                finalPrice: finalPrice,
                quantity: quantity,
                customization: {...currentCustomization}
            };
            
            // Cek apakah item dengan kustomisasi yang sama sudah ada di keranjang
            const existingIndex = cart.findIndex(i => 
                i.id === itemId && 
                i.customization.sugar === currentCustomization.sugar &&
                i.customization.ice === currentCustomization.ice &&
                i.customization.topping === currentCustomization.topping &&
                i.customization.utensils === currentCustomization.utensils &&
                i.customization.specialRequest === currentCustomization.specialRequest
            );
            
            if (existingIndex !== -1) {
                cart[existingIndex].quantity += quantity;
            } else {
                cart.push(cartItem);
            }
            
            updateCart();
            showNotification(`${item.name} ditambahkan ke keranjang`);
            
            // Tutup modal jika terbuka
            if (itemModal.classList.contains('active')) {
                itemModal.classList.remove('active');
                overlay.classList.remove('active');
            }
        }

        // Hapus item dari keranjang
        function removeFromCart(itemIndex) {
            cart.splice(itemIndex, 1);
            updateCart();
        }

        // Update kuantitas item
        function updateQuantity(itemIndex, newQuantity) {
            if (newQuantity < 1) {
                removeFromCart(itemIndex);
                return;
            }
            
            cart[itemIndex].quantity = newQuantity;
            updateCart();
        }

        // Update tampilan keranjang
        function updateCart() {
            // Update jumlah item di icon keranjang
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            cartCount.textContent = totalItems;
            
            // Update daftar item di sidebar
            cartItems.innerHTML = '';
            let subtotal = 0;
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Keranjang belanja kosong</p>';
            } else {
                cart.forEach((item, index) => {
                    const itemTotal = item.finalPrice * item.quantity;
                    subtotal += itemTotal;
                    
                    const cartItem = document.createElement('div');
                    cartItem.className = 'cart-item';
                    
                    let customizationText = '';
                    if (item.customization.sugar !== 'normal') {
                        customizationText += `Gula: ${item.customization.sugar}, `;
                    }
                    if (item.customization.ice !== 'normal') {
                        customizationText += `Es: ${item.customization.ice}, `;
                    }
                    if (item.customization.topping) {
                        customizationText += `Topping: ${item.customization.topping}, `;
                    }
                    if (item.customization.utensils) {
                        customizationText += `Perlengkapan: Ya, `;
                    }
                    if (item.customization.specialRequest) {
                        customizationText += `Request: ${item.customization.specialRequest}`;
                    }
                    
                    // Hapus koma di akhir jika ada
                    if (customizationText.endsWith(', ')) {
                        customizationText = customizationText.slice(0, -2);
                    }
                    
                    cartItem.innerHTML = `
                        <img src="${item.image}" alt="${item.name}">
                        <div class="cart-item-details">
                            <h4>${item.name}</h4>
                            <div class="cart-item-price">${formatRupiah(item.finalPrice)}</div>
                            ${customizationText ? `<div class="cart-item-customization">${customizationText}</div>` : ''}
                            <div class="cart-item-quantity">
                                <button class="quantity-btn minus" data-index="${index}">-</button>
                                <span class="quantity">${item.quantity}</span>
                                <button class="quantity-btn plus" data-index="${index}">+</button>
                                <button class="remove-item" data-index="${index}"><i class="fas fa-trash"></i></button>
                            </div>
                        </div>
                    `;
                    cartItems.appendChild(cartItem);
                });
                
                // Tambahkan event listener untuk tombol kuantitas dan hapus
                document.querySelectorAll('.quantity-btn.minus').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        updateQuantity(itemIndex, cart[itemIndex].quantity - 1);
                    });
                });
                
                document.querySelectorAll('.quantity-btn.plus').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        updateQuantity(itemIndex, cart[itemIndex].quantity + 1);
                    });
                });
                
                document.querySelectorAll('.remove-item').forEach(button => {
                    button.addEventListener('click', function() {
                        const itemIndex = parseInt(this.getAttribute('data-index'));
                        removeFromCart(itemIndex);
                    });
                });
            }
            
            // Update total
            cartTotal.textContent = formatRupiah(subtotal);
            
            // Update ringkasan pembayaran
            updatePaymentSummary();
        }

        // Update ringkasan pembayaran
        function updatePaymentSummary() {
            paymentSummary.innerHTML = '';
            let subtotal = 0;
            
            cart.forEach(item => {
                const itemTotal = item.finalPrice * item.quantity;
                subtotal += itemTotal;
                
                const summaryItem = document.createElement('div');
                summaryItem.className = 'summary-item';
                summaryItem.innerHTML = `
                    <span>${item.name} x${item.quantity}</span>
                    <span>${formatRupiah(itemTotal)}</span>
                `;
                paymentSummary.appendChild(summaryItem);
            });
            
            // Hitung biaya pengiriman
            const delivery = calculateDeliveryCost(subtotal, addressInput.value);
            const total = subtotal + delivery;
            
            deliveryCost.textContent = formatRupiah(delivery);
            paymentTotal.textContent = formatRupiah(total);
            
            // Update jumlah pembayaran di semua metode
            gopayAmount.textContent = formatRupiah(total);
            qrisAmount.textContent = formatRupiah(total);
            vaAmount.textContent = formatRupiah(total);
        }

        // Tampilkan notifikasi
        function showNotification(message) {
            // Buat elemen notifikasi
            const notification = document.createElement('div');
            notification.style.cssText = `
                position: fixed;
                top: 20px;
                right: 20px;
                background-color: var(--primary);
                color: white;
                padding: 15px 20px;
                border-radius: 5px;
                box-shadow: 0 4px 8px rgba(0,0,0,0.2);
                z-index: 1001;
                transition: transform 0.3s, opacity 0.3s;
                transform: translateX(100%);
                opacity: 0;
            `;
            notification.textContent = message;
            document.body.appendChild(notification);
            
            // Animasi masuk
            setTimeout(() => {
                notification.style.transform = 'translateX(0)';
                notification.style.opacity = '1';
            }, 100);
            
            // Animasi keluar setelah 3 detik
            setTimeout(() => {
                notification.style.transform = 'translateX(100%)';
                notification.style.opacity = '0';
                setTimeout(() => {
                    document.body.removeChild(notification);
                }, 300);
            }, 3000);
        }

        // Filter menu berdasarkan kategori
        function filterMenu(category) {
            if (category === 'all') {
                return menuItems;
            }
            return menuItems.filter(item => item.category === category);
        }

        // Navigasi halaman
        function navigateToPage(page) {
            // Sembunyikan semua halaman
            pages.forEach(p => p.classList.remove('active'));
            
            // Tampilkan halaman yang dipilih
            document.getElementById(page).classList.add('active');
            
            // Update navigasi aktif
            navLinks.forEach(link => {
                if (link.getAttribute('data-page') === page) {
                    link.classList.add('active');
                } else {
                    link.classList.remove('active');
                }
            });
            
            // Tutup keranjang jika terbuka
            cartSidebar.classList.remove('active');
            overlay.classList.remove('active');
            
            currentPage = page;
            
            // Inisialisasi peta jika navigasi ke tracking page
            if (page === 'tracking') {
                initMap();
            }
        }

        // Inisialisasi peta tracking
        function initMap() {
            const map = L.map('map').setView(hanamiCafeLocation, 12);
            
            L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                attribution: '© OpenStreetMap contributors'
            }).addTo(map);
            
            // Tambahkan marker untuk Hanami Cafe
            L.marker(hanamiCafeLocation)
                .addTo(map)
                .bindPopup('Hanami Cafe')
                .openPopup();
            
            // Simulasi lokasi driver (random sekitar Jakarta)
            const driverLocation = [
                hanamiCafeLocation[0] + (Math.random() - 0.5) * 0.1,
                hanamiCafeLocation[1] + (Math.random() - 0.5) * 0.1
            ];
            
            L.marker(driverLocation)
                .addTo(map)
                .bindPopup('Driver Location')
                .openPopup();
        }

        // Inisialisasi aplikasi
        function init() {
            // Render menu di halaman home (hanya 4 item pertama)
            renderMenuItems(homeMenuGrid, menuItems.slice(0, 4));
            
            // Render menu di halaman menu
            renderMenuItems(menuContainer, menuItems);
            
            // Event listener untuk icon keranjang
            cartIcon.addEventListener('click', () => {
                cartSidebar.classList.add('active');
                overlay.classList.add('active');
            });
            
            // Event listener untuk tutup keranjang
            closeCart.addEventListener('click', () => {
                cartSidebar.classList.remove('active');
                overlay.classList.remove('active');
            });
            
            overlay.addEventListener('click', () => {
                cartSidebar.classList.remove('active');
                overlay.classList.remove('active');
                itemModal.classList.remove('active');
            });
            
            // Event listener untuk tombol checkout
            checkoutBtn.addEventListener('click', () => {
                if (cart.length === 0) {
                    showNotification('Keranjang belanja kosong');
                    return;
                }
                navigateToPage('payment');
            });
            
            // Event listener untuk kembali ke keranjang
            backToCart.addEventListener('click', () => {
                navigateToPage('menu');
                cartSidebar.classList.add('active');
                overlay.classList.add('active');
            });
            
            // Event listener untuk konfirmasi pembayaran
            confirmPayment.addEventListener('click', () => {
                if (cart.length === 0) {
                    showNotification('Keranjang belanja kosong');
                    return;
                }
                
                // Validasi form
                if (!validateForm()) {
                    showNotification('Harap lengkapi informasi pengiriman dengan benar');
                    return;
                }
                
                // Data pesanan
                const orderData = {
                    orderNumber: 'HCM-' + Date.now(),
                    customer: {
                        name: nameInput.value.trim(),
                        phone: phoneInput.value.trim(),
                        email: emailInput.value.trim(),
                        address: addressInput.value.trim(),
                        notes: notesInput.value.trim()
                    },
                    items: cart,
                    delivery: {
                        method: 'GrabExpress',
                        cost: calculateDeliveryCost(
                            cart.reduce((sum, item) => sum + (item.finalPrice * item.quantity), 0),
                            addressInput.value.trim()
                        )
                    },
                    total: parseFloat(paymentTotal.textContent.replace(/[^\d]/g, '')),
                    timestamp: new Date().toISOString()
                };
                
                // Kirim notifikasi ke penjual
                sendSellerNotification(orderData);
                
                // Kirim notifikasi ke pelanggan
                const customerMessage = `Terima kasih! Pesanan Anda di Hanami Cafe (${orderData.orderNumber}) telah diterima. Estimasi pengiriman: 30-45 menit.`;
                sendCustomerNotification(orderData.customer.phone, customerMessage);
                
                // Simulasi pembayaran berhasil
                showNotification('Pembayaran berhasil! Pesanan Anda sedang diproses.');
                
                // Reset keranjang dan form
                cart = [];
                updateCart();
                nameInput.value = '';
                phoneInput.value = '';
                emailInput.value = '';
                addressInput.value = '';
                notesInput.value = '';
                
                // Navigasi ke halaman tracking setelah 3 detik
                setTimeout(() => {
                    navigateToPage('tracking');
                }, 3000);
            });
            
            // Event listener untuk filter kategori
            categoryButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Update tombol aktif
                    categoryButtons.forEach(btn => btn.classList.remove('active'));
                    this.classList.add('active');
                    
                    // Filter menu
                    const category = this.getAttribute('data-category');
                    const filteredItems = filterMenu(category);
                    renderMenuItems(menuContainer, filteredItems);
                });
            });
            
            // Event listener untuk navigasi
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const page = this.getAttribute('data-page');
                    navigateToPage(page);
                });
            });
            
            // Event listener untuk metode pembayaran
            paymentMethods.forEach(method => {
                method.addEventListener('click', function() {
                    paymentMethods.forEach(m => m.classList.remove('selected'));
                    this.classList.add('selected');
                    
                    // Tampilkan instruksi pembayaran yang sesuai
                    const methodType = this.getAttribute('data-method');
                    gopayInstructions.classList.remove('active');
                    qrisInstructions.classList.remove('active');
                    vaInstructions.classList.remove('active');
                    
                    if (methodType === 'gopay') {
                        gopayInstructions.classList.add('active');
                    } else if (methodType === 'qris') {
                        qrisInstructions.classList.add('active');
                    } else if (methodType === 'va') {
                        vaInstructions.classList.add('active');
                    }
                });
            });
            
            // Event listener untuk pilihan pengiriman
            deliveryOptions.forEach(option => {
                option.addEventListener('click', function() {
                    deliveryOptions.forEach(o => o.classList.remove('selected'));
                    this.classList.add('selected');
                    updatePaymentSummary(); // Update biaya pengiriman
                });
            });
            
            // Event listener untuk hubungi driver
            contactDriver.addEventListener('click', () => {
                // Simulasi panggilan telepon
                window.open('tel:+6281234567890');
            });
            
            // Event listener untuk modal
            modalClose.addEventListener('click', () => {
                itemModal.classList.remove('active');
                overlay.classList.remove('active');
            });
            
            // Event listener untuk option items
            optionItems.forEach(item => {
                item.addEventListener('click', function() {
                    const group = this.parentElement;
                    const optionType = group.previousElementSibling.textContent.toLowerCase();
                    
                    // Untuk topping dan perlengkapan, bisa pilih multiple
                    if (optionType.includes('topping') || optionType.includes('perlengkapan')) {
                        this.classList.toggle('selected');
                    } else {
                        // Untuk yang lain, hanya satu pilihan
                        group.querySelectorAll('.option-item').forEach(i => {
                            i.classList.remove('selected');
                        });
                        this.classList.add('selected');
                    }
                    
                    // Update currentCustomization berdasarkan jenis option
                    if (optionType.includes('gula')) {
                        currentCustomization.sugar = this.getAttribute('data-value');
                    } else if (optionType.includes('es')) {
                        currentCustomization.ice = this.getAttribute('data-value');
                    } else if (optionType.includes('topping')) {
                        if (this.classList.contains('selected')) {
                            currentCustomization.topping = this.getAttribute('data-value');
                        } else {
                            currentCustomization.topping = null;
                        }
                    } else if (optionType.includes('perlengkapan')) {
                        currentCustomization.utensils = this.classList.contains('selected') ? 
                            this.getAttribute('data-value') : null;
                    }
                });
            });
            
            // Event listener untuk special request character count
            specialRequest.addEventListener('input', function() {
                currentCustomization.specialRequest = this.value;
                charCount.textContent = this.value.length;
            });
            
            // Event listener untuk notes character count
            notesInput.addEventListener('input', function() {
                notesCharCount.textContent = this.value.length;
            });
            
            // Event listener untuk alamat pengiriman (update ongkir real-time)
            addressInput.addEventListener('input', function() {
                updatePaymentSummary();
            });
            
            // Event listener untuk quantity selector
            qtyMinus.addEventListener('click', () => {
                let qty = parseInt(qtyValue.textContent);
                if (qty > 1) {
                    qtyValue.textContent = qty - 1;
                }
            });
            
            qtyPlus.addEventListener('click', () => {
                let qty = parseInt(qtyValue.textContent);
                qtyValue.textContent = qty + 1;
            });
            
            // Event listener untuk tambah ke keranjang dari modal
            addToCartModal.addEventListener('click', () => {
                if (currentItem) {
                    const quantity = parseInt(qtyValue.textContent);
                    addToCart(currentItem.id, quantity);
                }
            });
        }

        // Jalankan inisialisasi saat DOM siap
        document.addEventListener('DOMContentLoaded', init);
    </script>
</body>
</html>
